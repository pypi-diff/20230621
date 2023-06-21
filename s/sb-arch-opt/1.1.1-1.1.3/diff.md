# Comparing `tmp/sb-arch-opt-1.1.1.tar.gz` & `tmp/sb-arch-opt-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb-arch-opt-1.1.1.tar", last modified: Mon Jun 12 13:48:21 2023, max compression
+gzip compressed data, was "sb-arch-opt-1.1.3.tar", last modified: Wed Jun 21 19:06:36 2023, max compression
```

## Comparing `sb-arch-opt-1.1.1.tar` & `sb-arch-opt-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:21.855454 sb-arch-opt-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-12 13:48:21.855454 sb-arch-opt-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:21.851454 sb-arch-opt-1.1.1/sb_arch_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/design_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/design_space_explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22217 2023-06-12 13:48:08.000000 sb-arch-opt-1.1.1/sb_arch_opt/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-12 13:48:08.000000 sb-arch-opt-1.1.1/sb_arch_opt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:21.855454 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:48:21.855454 sb-arch-opt-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-12 13:48:08.000000 sb-arch-opt-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.973551 sb-arch-opt-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt/algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/hc_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33800 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/infill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/arch_sbo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/botorch_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/hebo_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/md_mating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/pymoo_interface/storage_restart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/segomoe_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/smarty_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/tpe_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/tpe_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/tpe_interface/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.965551 sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/algo/trieste_interface/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24815 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/design_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/design_space_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/sb_arch_opt/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/gnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/hidden_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48482 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/md_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/problems_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/problems/turbofan_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22864 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/sb_arch_opt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_arch_sbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_hebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_pymoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_segomoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_smarty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_tpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/algo/test_trieste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.969551 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_gnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_hidden_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_md_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/problems/test_turbofan_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/test_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/test_design_space_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/sb_arch_opt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:06:36.961551 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 19:06:36.000000 sb-arch-opt-1.1.3/sb_arch_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:06:36.973551 sb-arch-opt-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-21 19:06:25.000000 sb-arch-opt-1.1.3/setup.py
```

### Comparing `sb-arch-opt-1.1.1/LICENSE` & `sb-arch-opt-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.1/PKG-INFO` & `sb-arch-opt-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb-arch-opt
-Version: 1.1.1
+Version: 1.1.3
 Summary: SBArchOpt: Surrogate-Based Architecture Optimization
 Author: Jasper Bussemaker
 Author-email: jasper.bussemaker@dlr.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
@@ -94,8 +94,10 @@
 If you require support for using SBArchOpt or want to collaborate, feel free to contact me.
 
 Contributions are appreciated too:
 - Fork the repository
 - Add your contributions to the fork
   - Update/add documentation
   - Add tests and make sure they pass (tests are run using `pytest`)
+- Read and sign the [Contributor License Agreement (CLA)](https://github.com/jbussemaker/SBArchOpt/blob/main/SBArchOpt%20DLR%20Individual%20Contributor%20License%20Agreement.docx)
+  , and send it to the project coordinator
 - Issue a pull request
```

### Comparing `sb-arch-opt-1.1.1/README.md` & `sb-arch-opt-1.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,8 +75,10 @@
 If you require support for using SBArchOpt or want to collaborate, feel free to contact me.
 
 Contributions are appreciated too:
 - Fork the repository
 - Add your contributions to the fork
   - Update/add documentation
   - Add tests and make sure they pass (tests are run using `pytest`)
+- Read and sign the [Contributor License Agreement (CLA)](https://github.com/jbussemaker/SBArchOpt/blob/main/SBArchOpt%20DLR%20Individual%20Contributor%20License%20Agreement.docx)
+  , and send it to the project coordinator
 - Issue a pull request
```

### Comparing `sb-arch-opt-1.1.1/sb_arch_opt/design_space.py` & `sb-arch-opt-1.1.3/sb_arch_opt/design_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
-Licensed under the GNU General Public License, Version 3.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    https://www.gnu.org/licenses/gpl-3.0.html.en
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+MIT License
 
 Copyright: (c) 2023, Deutsches Zentrum fuer Luft- und Raumfahrt e.V.
 Contact: jasper.bussemaker@dlr.de
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
 """
 import itertools
 import numpy as np
 import pandas as pd
 from typing import *
 from cached_property import cached_property
 from pymoo.core.variable import Variable, Real, Integer, Binary, Choice
@@ -362,14 +370,17 @@
 
     def quick_sample_discrete_x(self, n: int) -> Tuple[np.ndarray, np.ndarray]:
         """Sample n design vectors (also return is_active) without generating all design vectors first"""
 
         x, is_active = self._quick_sample_discrete_x(n)
         if x.shape[1] != self.n_var or is_active.shape[1] != self.n_var:
             raise RuntimeError(f'Inconsistent design vector dimensions: {x.shape[1]} != {self.n_var}')
+        if x.shape[0] > n:
+            x = x[:n, :]
+            is_active = is_active[:n, :]
         x = x.astype(float)  # Otherwise continuous variables cannot be imputed
 
         self.round_x_discrete(x)
         self.impute_x(x, is_active)
 
         return x, is_active
```

### Comparing `sb-arch-opt-1.1.1/sb_arch_opt/design_space_explicit.py` & `sb-arch-opt-1.1.3/sb_arch_opt/design_space_explicit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
-Licensed under the GNU General Public License, Version 3.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    https://www.gnu.org/licenses/gpl-3.0.html.en
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+MIT License
 
 Copyright: (c) 2023, Deutsches Zentrum fuer Luft- und Raumfahrt e.V.
 Contact: jasper.bussemaker@dlr.de
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
 """
 import numpy as np
 from typing import *
 from sb_arch_opt.design_space import ArchDesignSpace
 from pymoo.core.variable import Variable, Real, Integer, Choice
 
 from ConfigSpace.util import generate_grid, get_random_neighbor
```

### Comparing `sb-arch-opt-1.1.1/sb_arch_opt/pareto_front.py` & `sb-arch-opt-1.1.3/sb_arch_opt/pareto_front.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
-Licensed under the GNU General Public License, Version 3.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    https://www.gnu.org/licenses/gpl-3.0.html.en
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+MIT License
 
 Copyright: (c) 2023, Deutsches Zentrum fuer Luft- und Raumfahrt e.V.
 Contact: jasper.bussemaker@dlr.de
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
 """
 import os
 import re
 import pickle
 import hashlib
 import numpy as np
 from typing import *
```

### Comparing `sb-arch-opt-1.1.1/sb_arch_opt/problem.py` & `sb-arch-opt-1.1.3/sb_arch_opt/problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
-Licensed under the GNU General Public License, Version 3.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    https://www.gnu.org/licenses/gpl-3.0.html.en
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+MIT License
 
 Copyright: (c) 2023, Deutsches Zentrum fuer Luft- und Raumfahrt e.V.
 Contact: jasper.bussemaker@dlr.de
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
 """
 import numpy as np
 import pandas as pd
 from typing import List, Optional, Union, Tuple
 from pymoo.core.repair import Repair
 from pymoo.core.problem import Problem
 from pymoo.core.variable import Variable
```

### Comparing `sb-arch-opt-1.1.1/sb_arch_opt/sampling.py` & `sb-arch-opt-1.1.3/sb_arch_opt/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """
-Licensed under the GNU General Public License, Version 3.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    https://www.gnu.org/licenses/gpl-3.0.html.en
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+MIT License
 
 Copyright: (c) 2023, Deutsches Zentrum fuer Luft- und Raumfahrt e.V.
 Contact: jasper.bussemaker@dlr.de
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
 """
 import logging
 import warnings
 import numpy as np
 from typing import Optional, Tuple, List
 from scipy.stats.qmc import Sobol
 from scipy.spatial import distance
@@ -362,14 +370,18 @@
             if n_sel == n_in_group or not has_x_cont:
                 return np.concatenate([i_x_selected, np.arange(n_in_group)])
 
             # Pre-select all points once
             i_x_selected = np.concatenate([i_x_selected, np.arange(n_in_group)])
             n_sel = n_sel-n_in_group
 
+        if n_sel == 1:
+            i_x_take = choice_func(1, n_in_group, replace=False)
+            return np.concatenate([i_x_selected, i_x_take])
+
         # Randomly sample several times to get the best distribution of points
         i_x_tries = []
         metrics = []
         for _ in range(self.n_iter):
             i_x_try = choice_func(n_sel, n_in_group, replace=False)
             i_x_tries.append(i_x_try)
```

### Comparing `sb-arch-opt-1.1.1/sb_arch_opt/util.py` & `sb-arch-opt-1.1.3/sb_arch_opt/util.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.1/sb_arch_opt.egg-info/PKG-INFO` & `sb-arch-opt-1.1.3/sb_arch_opt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb-arch-opt
-Version: 1.1.1
+Version: 1.1.3
 Summary: SBArchOpt: Surrogate-Based Architecture Optimization
 Author: Jasper Bussemaker
 Author-email: jasper.bussemaker@dlr.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
@@ -94,8 +94,10 @@
 If you require support for using SBArchOpt or want to collaborate, feel free to contact me.
 
 Contributions are appreciated too:
 - Fork the repository
 - Add your contributions to the fork
   - Update/add documentation
   - Add tests and make sure they pass (tests are run using `pytest`)
+- Read and sign the [Contributor License Agreement (CLA)](https://github.com/jbussemaker/SBArchOpt/blob/main/SBArchOpt%20DLR%20Individual%20Contributor%20License%20Agreement.docx)
+  , and send it to the project coordinator
 - Issue a pull request
```

