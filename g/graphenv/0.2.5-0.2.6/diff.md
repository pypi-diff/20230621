# Comparing `tmp/graphenv-0.2.5.tar.gz` & `tmp/graphenv-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphenv-0.2.5.tar", last modified: Fri Apr 21 21:33:33 2023, max compression
+gzip compressed data, was "graphenv-0.2.6.tar", last modified: Wed Jun 21 19:01:30 2023, max compression
```

## Comparing `graphenv-0.2.5.tar` & `graphenv-0.2.6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.491210 graphenv-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 21:33:22.000000 graphenv-0.2.5/.envrc
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 21:33:22.000000 graphenv-0.2.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.479210 graphenv-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-21 21:33:22.000000 graphenv-0.2.5/.github/workflows/build_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-21 21:33:22.000000 graphenv-0.2.5/.github/workflows/draft_pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-21 21:33:22.000000 graphenv-0.2.5/.github/workflows/run_tests_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-21 21:33:22.000000 graphenv-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 21:33:22.000000 graphenv-0.2.5/.lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-21 21:33:22.000000 graphenv-0.2.5/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-21 21:33:22.000000 graphenv-0.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-21 21:33:22.000000 graphenv-0.2.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-21 21:33:22.000000 graphenv-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-21 21:33:33.491210 graphenv-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-21 21:33:22.000000 graphenv-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-21 21:33:22.000000 graphenv-0.2.5/codemeta.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/devtools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/devtools/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-04-21 21:33:22.000000 graphenv-0.2.5/devtools/aws/example-tsp.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/devtools/conda-envs/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-21 21:33:22.000000 graphenv-0.2.5/devtools/conda-envs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-21 21:33:22.000000 graphenv-0.2.5/devtools/sphinx.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/requirements_for_docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/_templates/custom-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/docs/source/about/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.483210 graphenv-0.2.5/docs/source/background/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/background/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.487210 graphenv-0.2.5/docs/source/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)   828456 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/cloud/ray-dashboard-example.png
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/cloud/tsp_on_aws.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.487210 graphenv-0.2.5/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    24144 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/hallway.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/hallway_test_tf.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/hallway_test_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.487210 graphenv-0.2.5/docs/source/examples/img/
--rw-r--r--   0 runner    (1001) docker     (123)    40829 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/img/graphenv.png
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/img/hallway-flat.png
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/img/hallway-graph.png
--rw-r--r--   0 runner    (1001) docker     (123)    53545 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/img/hallway.pptx
--rw-r--r--   0 runner    (1001) docker     (123)    78709 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/img/tsp-graph.png
--rw-r--r--   0 runner    (1001) docker     (123)    82816 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/movie.mp4
--rw-r--r--   0 runner    (1001) docker     (123)    56198 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/movie.webm
--rw-r--r--   0 runner    (1001) docker     (123)   295273 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/tsp_docs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    44717 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/tsp_env.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/examples/tune.rst
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-21 21:33:22.000000 graphenv-0.2.5/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.479210 graphenv-0.2.5/experiments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.487210 graphenv-0.2.5/experiments/hallway/
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-21 21:33:22.000000 graphenv-0.2.5/experiments/hallway/custom_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-21 21:33:22.000000 graphenv-0.2.5/experiments/hallway/run_hallway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.487210 graphenv-0.2.5/experiments/tsp/
--rwxr-xr-x   0 runner    (1001) docker     (123)      464 2023-04-21 21:33:22.000000 graphenv-0.2.5/experiments/tsp/run-tsp.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-21 21:33:22.000000 graphenv-0.2.5/experiments/tsp/run_tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-21 21:33:22.000000 graphenv-0.2.5/experiments/tsp/run_tsp_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-04-21 21:33:22.000000 graphenv-0.2.5/experiments/tsp/tsp_profiling.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-04-21 21:33:22.000000 graphenv-0.2.5/experiments/tsp/untrained_model_sampling.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.491210 graphenv-0.2.5/graphenv/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 21:33:33.000000 graphenv-0.2.5/graphenv/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.491210 graphenv-0.2.5/graphenv/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.491210 graphenv-0.2.5/graphenv/examples/hallway/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/hallway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/hallway/hallway_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/hallway/hallway_model_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/hallway/hallway_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.491210 graphenv-0.2.5/graphenv/examples/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/tsp/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/tsp/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/tsp/tsp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/tsp/tsp_nfp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/tsp/tsp_nfp_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/tsp/tsp_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/examples/tsp/tsp_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/graph_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/graph_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/graph_model_bellman_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-21 21:33:22.000000 graphenv-0.2.5/graphenv/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.491210 graphenv-0.2.5/graphenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-21 21:33:33.000000 graphenv-0.2.5/graphenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-21 21:33:33.000000 graphenv-0.2.5/graphenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:33:33.000000 graphenv-0.2.5/graphenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-21 21:33:33.000000 graphenv-0.2.5/graphenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 21:33:33.000000 graphenv-0.2.5/graphenv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.491210 graphenv-0.2.5/joss/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-21 21:33:22.000000 graphenv-0.2.5/joss/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-21 21:33:22.000000 graphenv-0.2.5/joss/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-04-21 21:33:22.000000 graphenv-0.2.5/joss/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-21 21:33:22.000000 graphenv-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-21 21:33:33.491210 graphenv-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 21:33:22.000000 graphenv-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:33.491210 graphenv-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:33:22.000000 graphenv-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-21 21:33:22.000000 graphenv-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-21 21:33:22.000000 graphenv-0.2.5/tests/test_graph_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-21 21:33:22.000000 graphenv-0.2.5/tests/test_hallway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-21 21:33:22.000000 graphenv-0.2.5/tests/test_tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.866576 graphenv-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 19:01:18.000000 graphenv-0.2.6/.envrc
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 19:01:18.000000 graphenv-0.2.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.842576 graphenv-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.846576 graphenv-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-21 19:01:18.000000 graphenv-0.2.6/.github/workflows/build_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-21 19:01:18.000000 graphenv-0.2.6/.github/workflows/draft_pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-21 19:01:18.000000 graphenv-0.2.6/.github/workflows/run_tests_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-21 19:01:18.000000 graphenv-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-21 19:01:18.000000 graphenv-0.2.6/.lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-21 19:01:18.000000 graphenv-0.2.6/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-21 19:01:18.000000 graphenv-0.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-21 19:01:18.000000 graphenv-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-21 19:01:18.000000 graphenv-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-21 19:01:30.866576 graphenv-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-21 19:01:18.000000 graphenv-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-21 19:01:18.000000 graphenv-0.2.6/codemeta.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.850576 graphenv-0.2.6/devtools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.850576 graphenv-0.2.6/devtools/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-06-21 19:01:18.000000 graphenv-0.2.6/devtools/aws/example-tsp.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.850576 graphenv-0.2.6/devtools/conda-envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 19:01:18.000000 graphenv-0.2.6/devtools/conda-envs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 19:01:18.000000 graphenv-0.2.6/devtools/sphinx.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.850576 graphenv-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/requirements_for_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.850576 graphenv-0.2.6/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.850576 graphenv-0.2.6/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/_templates/custom-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.850576 graphenv-0.2.6/docs/source/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.850576 graphenv-0.2.6/docs/source/background/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/background/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.854576 graphenv-0.2.6/docs/source/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)   828456 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/cloud/ray-dashboard-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/cloud/tsp_on_aws.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.854576 graphenv-0.2.6/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    24144 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/hallway.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/hallway_test_tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/hallway_test_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.858576 graphenv-0.2.6/docs/source/examples/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    40829 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/img/graphenv.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/img/hallway-flat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/img/hallway-graph.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53545 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/img/hallway.pptx
+-rw-r--r--   0 runner    (1001) docker     (123)    78709 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/img/tsp-graph.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82816 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/movie.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)    56198 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/movie.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   295273 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/tsp_docs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    44717 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/tsp_env.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/examples/tune.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 19:01:18.000000 graphenv-0.2.6/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.842576 graphenv-0.2.6/experiments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.858576 graphenv-0.2.6/experiments/hallway/
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-21 19:01:18.000000 graphenv-0.2.6/experiments/hallway/custom_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-21 19:01:18.000000 graphenv-0.2.6/experiments/hallway/run_hallway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.858576 graphenv-0.2.6/experiments/tsp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      464 2023-06-21 19:01:18.000000 graphenv-0.2.6/experiments/tsp/run-tsp.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-21 19:01:18.000000 graphenv-0.2.6/experiments/tsp/run_tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-21 19:01:18.000000 graphenv-0.2.6/experiments/tsp/run_tsp_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-21 19:01:18.000000 graphenv-0.2.6/experiments/tsp/tsp_profiling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-06-21 19:01:18.000000 graphenv-0.2.6/experiments/tsp/untrained_model_sampling.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.862576 graphenv-0.2.6/graphenv/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 19:01:30.000000 graphenv-0.2.6/graphenv/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.862576 graphenv-0.2.6/graphenv/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.862576 graphenv-0.2.6/graphenv/examples/hallway/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/hallway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/hallway/hallway_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/hallway/hallway_model_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/hallway/hallway_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.866576 graphenv-0.2.6/graphenv/examples/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/tsp/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/tsp/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/tsp/tsp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/tsp/tsp_nfp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/tsp/tsp_nfp_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/tsp/tsp_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/examples/tsp/tsp_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/graph_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/graph_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/graph_model_bellman_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-21 19:01:18.000000 graphenv-0.2.6/graphenv/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.862576 graphenv-0.2.6/graphenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-21 19:01:30.000000 graphenv-0.2.6/graphenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-21 19:01:30.000000 graphenv-0.2.6/graphenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:01:30.000000 graphenv-0.2.6/graphenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 19:01:30.000000 graphenv-0.2.6/graphenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 19:01:30.000000 graphenv-0.2.6/graphenv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.866576 graphenv-0.2.6/joss/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 19:01:18.000000 graphenv-0.2.6/joss/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-21 19:01:18.000000 graphenv-0.2.6/joss/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-21 19:01:18.000000 graphenv-0.2.6/joss/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 19:01:18.000000 graphenv-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-21 19:01:30.866576 graphenv-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 19:01:18.000000 graphenv-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:30.866576 graphenv-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:01:18.000000 graphenv-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-21 19:01:18.000000 graphenv-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-21 19:01:18.000000 graphenv-0.2.6/tests/test_graph_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-21 19:01:18.000000 graphenv-0.2.6/tests/test_hallway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-21 19:01:18.000000 graphenv-0.2.6/tests/test_tsp.py
```

### Comparing `graphenv-0.2.5/.github/workflows/build_docs.yml` & `graphenv-0.2.6/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/.github/workflows/draft_pdf.yml` & `graphenv-0.2.6/.github/workflows/draft_pdf.yml`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/.github/workflows/run_tests_and_deploy.yml` & `graphenv-0.2.6/.github/workflows/run_tests_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/.gitignore` & `graphenv-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/.zenodo.json` & `graphenv-0.2.6/.zenodo.json`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/CODE_OF_CONDUCT.md` & `graphenv-0.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/CONTRIBUTING.md` & `graphenv-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/LICENSE` & `graphenv-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/PKG-INFO` & `graphenv-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphenv
-Version: 0.2.5
+Version: 0.2.6
 Summary: Reinforcement learning on directed graphs
 License: BSD 3-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: torch
```

### Comparing `graphenv-0.2.5/README.md` & `graphenv-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/codemeta.json` & `graphenv-0.2.6/codemeta.json`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/devtools/aws/example-tsp.yml` & `graphenv-0.2.6/devtools/aws/example-tsp.yml`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/Makefile` & `graphenv-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/make.bat` & `graphenv-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/_templates/custom-class-template.rst` & `graphenv-0.2.6/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/_templates/custom-module-template.rst` & `graphenv-0.2.6/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/api.rst` & `graphenv-0.2.6/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/background/introduction.rst` & `graphenv-0.2.6/docs/source/background/introduction.rst`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/cloud/ray-dashboard-example.png` & `graphenv-0.2.6/docs/source/cloud/ray-dashboard-example.png`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/cloud/tsp_on_aws.ipynb` & `graphenv-0.2.6/docs/source/cloud/tsp_on_aws.ipynb`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/conf.py` & `graphenv-0.2.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/hallway.ipynb` & `graphenv-0.2.6/docs/source/examples/hallway.ipynb`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/hallway_test_tf.py` & `graphenv-0.2.6/docs/source/examples/hallway_test_tf.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/hallway_test_torch.py` & `graphenv-0.2.6/docs/source/examples/hallway_test_torch.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/img/graphenv.png` & `graphenv-0.2.6/docs/source/examples/img/graphenv.png`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/img/hallway-flat.png` & `graphenv-0.2.6/docs/source/examples/img/hallway-flat.png`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/img/hallway-graph.png` & `graphenv-0.2.6/docs/source/examples/img/hallway-graph.png`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/img/hallway.pptx` & `graphenv-0.2.6/docs/source/examples/img/hallway.pptx`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/img/tsp-graph.png` & `graphenv-0.2.6/docs/source/examples/img/tsp-graph.png`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/movie.mp4` & `graphenv-0.2.6/docs/source/examples/movie.mp4`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/movie.webm` & `graphenv-0.2.6/docs/source/examples/movie.webm`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/tsp_docs.ipynb` & `graphenv-0.2.6/docs/source/examples/tsp_docs.ipynb`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/tsp_env.ipynb` & `graphenv-0.2.6/docs/source/examples/tsp_env.ipynb`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/examples/tune.rst` & `graphenv-0.2.6/docs/source/examples/tune.rst`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/docs/source/index.rst` & `graphenv-0.2.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/experiments/hallway/custom_env.py` & `graphenv-0.2.6/experiments/hallway/custom_env.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/experiments/hallway/run_hallway.py` & `graphenv-0.2.6/experiments/hallway/run_hallway.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/experiments/tsp/run_tsp.py` & `graphenv-0.2.6/experiments/tsp/run_tsp.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/experiments/tsp/run_tsp_aws.py` & `graphenv-0.2.6/experiments/tsp/run_tsp_aws.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/experiments/tsp/tsp_profiling.ipynb` & `graphenv-0.2.6/experiments/tsp/tsp_profiling.ipynb`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/experiments/tsp/untrained_model_sampling.ipynb` & `graphenv-0.2.6/experiments/tsp/untrained_model_sampling.ipynb`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/hallway/hallway_model.py` & `graphenv-0.2.6/graphenv/examples/hallway/hallway_model.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/hallway/hallway_model_torch.py` & `graphenv-0.2.6/graphenv/examples/hallway/hallway_model_torch.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/hallway/hallway_state.py` & `graphenv-0.2.6/graphenv/examples/hallway/hallway_state.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/tsp/README.md` & `graphenv-0.2.6/graphenv/examples/tsp/README.md`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/tsp/graph_utils.py` & `graphenv-0.2.6/graphenv/examples/tsp/graph_utils.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/tsp/tsp_model.py` & `graphenv-0.2.6/graphenv/examples/tsp/tsp_model.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/tsp/tsp_nfp_model.py` & `graphenv-0.2.6/graphenv/examples/tsp/tsp_nfp_model.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/tsp/tsp_nfp_state.py` & `graphenv-0.2.6/graphenv/examples/tsp/tsp_nfp_state.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/tsp/tsp_preprocessor.py` & `graphenv-0.2.6/graphenv/examples/tsp/tsp_preprocessor.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/examples/tsp/tsp_state.py` & `graphenv-0.2.6/graphenv/examples/tsp/tsp_state.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/graph_env.py` & `graphenv-0.2.6/graphenv/graph_env.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/graph_model.py` & `graphenv-0.2.6/graphenv/graph_model.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv/vertex.py` & `graphenv-0.2.6/graphenv/vertex.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/graphenv.egg-info/PKG-INFO` & `graphenv-0.2.6/graphenv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphenv
-Version: 0.2.5
+Version: 0.2.6
 Summary: Reinforcement learning on directed graphs
 License: BSD 3-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: torch
```

### Comparing `graphenv-0.2.5/graphenv.egg-info/SOURCES.txt` & `graphenv-0.2.6/graphenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/joss/paper.bib` & `graphenv-0.2.6/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/joss/paper.md` & `graphenv-0.2.6/joss/paper.md`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/setup.cfg` & `graphenv-0.2.6/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 install_requires = 
 	networkx==3.0
 	ray[tune,rllib]==2.3.1
+	tensorboardX==2.6.0
 	numpy<1.24.0
 	tqdm==4.64.1
 	matplotlib
 
 [options.extras_require]
 tensorflow = tensorflow
 torch = torch
```

### Comparing `graphenv-0.2.5/tests/conftest.py` & `graphenv-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/tests/test_graph_model_utils.py` & `graphenv-0.2.6/tests/test_graph_model_utils.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/tests/test_hallway.py` & `graphenv-0.2.6/tests/test_hallway.py`

 * *Files identical despite different names*

### Comparing `graphenv-0.2.5/tests/test_tsp.py` & `graphenv-0.2.6/tests/test_tsp.py`

 * *Files identical despite different names*

