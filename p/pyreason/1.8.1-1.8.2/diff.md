# Comparing `tmp/pyreason-1.8.1.tar.gz` & `tmp/pyreason-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.8.1.tar", last modified: Fri Jun 16 11:07:41 2023, max compression
+gzip compressed data, was "pyreason-1.8.2.tar", last modified: Wed Jun 21 14:05:50 2023, max compression
```

## Comparing `pyreason-1.8.1.tar` & `pyreason-1.8.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.582791 pyreason-1.8.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-16 11:07:31.000000 pyreason-1.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 11:07:31.000000 pyreason-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-16 11:07:41.582791 pyreason-1.8.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-06-16 11:07:31.000000 pyreason-1.8.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    27957 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/facts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/facts/fact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    74858 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/rule_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:07:41.582791 pyreason-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-16 11:07:31.000000 pyreason-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-16 11:07:31.000000 pyreason-1.8.1/tests/test_hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.326357 pyreason-1.8.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-21 14:05:37.000000 pyreason-1.8.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 14:05:37.000000 pyreason-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-21 14:05:50.326357 pyreason-1.8.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-06-21 14:05:37.000000 pyreason-1.8.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.318357 pyreason-1.8.2/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.318357 pyreason-1.8.2/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.318357 pyreason-1.8.2/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28008 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    75254 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.326357 pyreason-1.8.2/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4587 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.318357 pyreason-1.8.2/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:05:50.326357 pyreason-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 14:05:37.000000 pyreason-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.326357 pyreason-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-21 14:05:37.000000 pyreason-1.8.2/tests/test_hello_world.py
```

### Comparing `pyreason-1.8.1/LICENSE.md` & `pyreason-1.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/PKG-INFO` & `pyreason-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.1
+Version: 1.8.2
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.1/README.md` & `pyreason-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/__init__.py` & `pyreason-1.8.2/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.8.2/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.8.2/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.8.2/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/pyreason.py` & `pyreason-1.8.2/pyreason/pyreason.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,15 +442,15 @@
     :param file_path: Path to the text file containing rules
     :type file_path: str
     :param infer_edges: Whether to infer edges on these rules if an edge doesn't exist between head variables and the body of the rule is satisfied
     :type infer_edges: bool
     :return: None
     """
     with open(file_path, 'r') as file:
-        rules = [line.rstrip() for line in file]
+        rules = [line.rstrip() for line in file if line.rstrip() != '' and line.rstrip()[0] != '#']
 
     rule_offset = 0 if __rules is None else len(__rules)
     for i, r in enumerate(rules):
         add_rule(r, f'rule_{i+rule_offset}', infer_edges)
 
 
 def add_fact(pyreason_fact: Fact) -> None:
```

### Comparing `pyreason-1.8.1/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.8.2/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/args.py` & `pyreason-1.8.2/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/components/world.py` & `pyreason-1.8.2/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/diffuse.py` & `pyreason-1.8.2/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/facts/fact.py` & `pyreason-1.8.2/pyreason/scripts/facts/fact.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.8.2/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/facts/fact_node.py` & `pyreason-1.8.2/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.8.2/pyreason/scripts/interpretation/interpretation.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,14 +442,16 @@
 							elif not immediate_edge_rule_fire and u:
 								immediate_rule_applied = True
 								break
 
 				# Remove from rules to be applied and edges to be applied lists after coming out from loop
 				rules_to_be_applied_node[:] = numba.typed.List([rules_to_be_applied_node[i] for i in range(len(rules_to_be_applied_node)) if i not in rules_to_remove_idx])
 				edges_to_be_added_node_rule[:] = numba.typed.List([edges_to_be_added_node_rule[i] for i in range(len(edges_to_be_added_node_rule)) if i not in rules_to_remove_idx])
+				if atom_trace:
+					rules_to_be_applied_node_trace[:] = numba.typed.List([rules_to_be_applied_node_trace[i] for i in range(len(rules_to_be_applied_node_trace)) if i not in rules_to_remove_idx])
 
 				# Edges
 				rules_to_remove_idx.clear()
 				for idx, i in enumerate(rules_to_be_applied_edge):
 					# If we broke from above loop to apply more rules, then break from here
 					if immediate_rule_applied and not immediate_edge_rule_fire:
 						break
@@ -529,14 +531,16 @@
 							elif not immediate_edge_rule_fire and u:
 								immediate_rule_applied = True
 								break
 
 				# Remove from rules to be applied and edges to be applied lists after coming out from loop
 				rules_to_be_applied_edge[:] = numba.typed.List([rules_to_be_applied_edge[i] for i in range(len(rules_to_be_applied_edge)) if i not in rules_to_remove_idx])
 				edges_to_be_added_edge_rule[:] = numba.typed.List([edges_to_be_added_edge_rule[i] for i in range(len(edges_to_be_added_edge_rule)) if i not in rules_to_remove_idx])
+				if atom_trace:
+					rules_to_be_applied_edge_trace[:] = numba.typed.List([rules_to_be_applied_edge_trace[i] for i in range(len(rules_to_be_applied_edge_trace)) if i not in rules_to_remove_idx])
 
 				# Fixed point
 				# if update or immediate_node_rule_fire or immediate_edge_rule_fire or immediate_rule_applied:
 				if update:
 					# Increase fp operator count only if not an immediate rule
 					if not (immediate_node_rule_fire or immediate_edge_rule_fire):
 						fp_cnt += 1
```

### Comparing `pyreason-1.8.1/pyreason/scripts/interval/interval.py` & `pyreason-1.8.2/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/program/program.py` & `pyreason-1.8.2/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/rules/rule.py` & `pyreason-1.8.2/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/utils/filter.py` & `pyreason-1.8.2/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.8.2/pyreason/scripts/utils/graphml_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,80 +7,87 @@
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 
 
 class GraphmlParser:
     def __init__(self):
         self.graph = None
         self.non_fluent_facts = None
-        
+
     def parse_graph(self, graph_path, reverse):
         self.graph = nx.read_graphml(graph_path)
         if reverse:
             self.graph = self.graph.reverse()
 
         return self.graph
 
     def parse_graph_attributes(self, static_facts):
         facts_node = numba.typed.List.empty_list(fact_node.fact_type)
         facts_edge = numba.typed.List.empty_list(fact_edge.fact_type)
-        specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.string))
-        specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.Tuple((numba.types.string, numba.types.string))))
+        specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type,
+                                                      value_type=numba.types.ListType(numba.types.string))
+        specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(
+            numba.types.Tuple((numba.types.string, numba.types.string))))
         for n in self.graph.nodes:
             for key, value in self.graph.nodes[n].items():
                 # IF attribute is a float or int and it is less than 1, then make it a bound, else make it a label
-                if isinstance(value, (float, int)) and value<=1 and value>=0:
+                if (isinstance(value, (float, int)) and 1 >= value >= 0) or (
+                        isinstance(value, str) and value.replace('.', '').isdigit() and 1 >= float(value) >= 0):
                     l = str(key)
                     l_bnd = float(value)
                     u_bnd = 1
                 else:
                     l = f'{key}-{value}'
                     l_bnd = 1
                     u_bnd = 1
                 if isinstance(value, str):
                     bnd_str = value.split(',')
-                    if len(bnd_str)==2:
+                    if len(bnd_str) == 2:
                         try:
                             low = int(bnd_str[0])
                             up = int(bnd_str[1])
-                            if low<=1 and low>=0 and up<=1 and up>=0:
+                            if 1 >= low >= 0 and 1 >= up >= 0:
                                 l_bnd = low
                                 u_bnd = up
                                 l = str(key)
                         except:
                             pass
-                
+
                 if label.Label(l) not in specific_node_labels.keys():
                     specific_node_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.string)
                 specific_node_labels[label.Label(l)].append(n)
-                f = fact_node.Fact('graph-attribute-fact', n, label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
+                f = fact_node.Fact('graph-attribute-fact', n, label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0,
+                                   static=static_facts)
                 facts_node.append(f)
         for e in self.graph.edges:
             for key, value in self.graph.edges[e].items():
                 # IF attribute is a float or int and it is less than 1, then make it a bound, else make it a label
-                if isinstance(value, (float, int)) and value<=1 and value>=0:
+                if (isinstance(value, (float, int)) and 1 >= value >= 0) or (
+                        isinstance(value, str) and value.replace('.', '').isdigit() and 1 >= float(value) >= 0):
                     l = str(key)
                     l_bnd = float(value)
                     u_bnd = 1
                 else:
                     l = f'{key}-{value}'
                     l_bnd = 1
                     u_bnd = 1
                 if isinstance(value, str):
                     bnd_str = value.split(',')
-                    if len(bnd_str)==2:
+                    if len(bnd_str) == 2:
                         try:
                             low = int(bnd_str[0])
                             up = int(bnd_str[1])
-                            if low<=1 and low>=0 and up<=1 and up>=0:
+                            if 1 >= low >= 0 and 1 >= up >= 0:
                                 l_bnd = low
                                 u_bnd = up
                                 l = str(key)
                         except:
                             pass
 
                 if label.Label(l) not in specific_edge_labels.keys():
-                    specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.string)))
+                    specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(
+                        numba.types.Tuple((numba.types.string, numba.types.string)))
                 specific_edge_labels[label.Label(l)].append((e[0], e[1]))
-                f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
+                f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd),
+                                   0, 0, static=static_facts)
                 facts_edge.append(f)
 
         return facts_node, facts_edge, specific_node_labels, specific_edge_labels
```

### Comparing `pyreason-1.8.1/pyreason/scripts/utils/output.py` & `pyreason-1.8.2/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/utils/plotter.py` & `pyreason-1.8.2/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/utils/rule_parser.py` & `pyreason-1.8.2/pyreason/scripts/utils/rule_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         assert len(head_variables) == 2, 'Cannot infer edges with a node rule. There have to be two variables in the head'
         var = '__target' if head_variables[0] == head_variables[1] else head_variables[1]
         edges = ('__target', var, target)
     else:
         edges = ('', '', label.Label(''))
 
     # Bound to set atom if rule fires
-    bnd = interval.closed(1, 1)
+    bnd = interval.closed(*target_bound)
     ann_fn = ''
     ann_label = label.Label('')
 
     weights = np.ones(len(body_predicates), dtype=np.float64)
     weights = np.append(weights, 0)
 
     r = rule.Rule(name, rule_type, target, numba.types.uint16(t), clauses, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule)
```

### Comparing `pyreason-1.8.1/pyreason/scripts/utils/visuals.py` & `pyreason-1.8.2/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.8.2/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/pyreason.egg-info/PKG-INFO` & `pyreason-1.8.2/pyreason.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.1
+Version: 1.8.2
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.1/pyreason.egg-info/SOURCES.txt` & `pyreason-1.8.2/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.1/setup.py` & `pyreason-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyreason',
-    version='1.8.1',
+    version='1.8.2',
     author='Dyuman Aditya',
     author_email='dyuman.aditya@gmail.com',
     description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lab-v2/pyreason',
     license='BSD 3-clause',
```

### Comparing `pyreason-1.8.1/tests/test_hello_world.py` & `pyreason-1.8.2/tests/test_hello_world.py`

 * *Files identical despite different names*

