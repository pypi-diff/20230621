# Comparing `tmp/jaxonnxruntime-0.0.2.tar.gz` & `tmp/jaxonnxruntime-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxonnxruntime-0.0.2.tar", last modified: Fri May 19 23:45:43 2023, max compression
+gzip compressed data, was "jaxonnxruntime-0.1.0.tar", last modified: Tue Jun 20 22:59:15 2023, max compression
```

## Comparing `jaxonnxruntime-0.0.2.tar` & `jaxonnxruntime-0.1.0.tar`

### file list

```diff
@@ -1,95 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.311497 jaxonnxruntime-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.291496 jaxonnxruntime-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.295496 jaxonnxruntime-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-19 23:45:43.311497 jaxonnxruntime-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.299496 jaxonnxruntime-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.291496 jaxonnxruntime-0.0.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.299496 jaxonnxruntime-0.0.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/docs/_static/css/jaxonnxruntime_theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.299496 jaxonnxruntime-0.0.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/docs/examples/jaxonnxruntime-python-api.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.295496 jaxonnxruntime-0.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.299496 jaxonnxruntime-0.0.2/examples/imagenet/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/examples/imagenet/imagenet_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.299496 jaxonnxruntime-0.0.2/jaxonnxruntime/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/call_onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.299496 jaxonnxruntime-0.0.2/jaxonnxruntime/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/core/onnx_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/core/onnx_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.311497 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/abs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/averagepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/batchnormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/constantofshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/div.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/gemm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/globalaveragepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/maxpool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/mul.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/nonzero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/pow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/reducemax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/reducemean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/reducesum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/sqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/jaxonnxruntime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.299496 jaxonnxruntime-0.0.2/jaxonnxruntime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-19 23:45:43.000000 jaxonnxruntime-0.0.2/jaxonnxruntime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-19 23:45:43.000000 jaxonnxruntime-0.0.2/jaxonnxruntime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:45:43.000000 jaxonnxruntime-0.0.2/jaxonnxruntime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-19 23:45:43.000000 jaxonnxruntime-0.0.2/jaxonnxruntime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 23:45:43.000000 jaxonnxruntime-0.0.2/jaxonnxruntime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:45:43.311497 jaxonnxruntime-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.311497 jaxonnxruntime-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tests/call_onnx_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.311497 jaxonnxruntime-0.0.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tests/core/handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tests/core/onnx_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tests/core/onnx_node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tests/onnx_models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tests/onnx_ops_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tests/run_all_tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:45:43.311497 jaxonnxruntime-0.0.2/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tools/analyze_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-19 23:45:19.000000 jaxonnxruntime-0.0.2/tools/op_code_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.935574 jaxonnxruntime-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.935574 jaxonnxruntime-0.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/_static/css/jaxonnxruntime_theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/examples/jaxonnxruntime-python-api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.935574 jaxonnxruntime-0.1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.939574 jaxonnxruntime-0.1.0/examples/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/examples/imagenet/imagenet_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.943574 jaxonnxruntime-0.1.0/jaxonnxruntime/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/call_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.943574 jaxonnxruntime-0.1.0/jaxonnxruntime/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/abs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/averagepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/batchnormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/constantofshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/div.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/gemm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/globalaveragepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/if_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/less.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/lessorequal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/lrn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/maxpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/mul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/nonzero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/or_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/pow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducemax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducemean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducesum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/jaxonnxruntime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.943574 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 22:59:15.000000 jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/call_onnx_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/core/handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/core/onnx_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/core/onnx_node_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/tests/onnx_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/onnx_ops/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/onnx_ops/onehot_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/onnx_ops_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tests/run_all_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:15.955574 jaxonnxruntime-0.1.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tools/analyze_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-20 22:58:52.000000 jaxonnxruntime-0.1.0/tools/op_code_generator.py
```

### Comparing `jaxonnxruntime-0.0.2/.github/workflows/build.yml` & `jaxonnxruntime-0.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/.github/workflows/pythonpublish.yml` & `jaxonnxruntime-0.1.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/.pre-commit-config.yaml` & `jaxonnxruntime-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/LICENSE` & `jaxonnxruntime-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/docs/conf.py` & `jaxonnxruntime-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/docs/examples/jaxonnxruntime-python-api.py` & `jaxonnxruntime-0.1.0/docs/examples/jaxonnxruntime-python-api.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/docs/index.rst` & `jaxonnxruntime-0.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/examples/imagenet/imagenet_main.py` & `jaxonnxruntime-0.1.0/examples/imagenet/imagenet_main.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 # limitations under the License.
 
 """Quick example how to run resnet50 with jaxonnxruntime."""
 
 # Users can do more experiments based on flax resnet50 examples
 # https://github.com/google/flax/tree/main/examples/imagenet
 
+import functools
 import logging
+from typing import Any
 
 from absl import app
 from absl import flags
 import jax
 from jax import numpy as jnp
+from jax.experimental import jax2tf
 from jaxonnxruntime import backend as JaxBackend
 from jaxonnxruntime import call_onnx
 import numpy as np
-from orbax.export import ExportManager
-from orbax.export import JaxModule
-from orbax.export import ServingConfig
+from orbax import export as orbax_export
 import tensorflow as tf
 
-
 import onnx
 from onnx import hub
-
+from onnx import shape_inference
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string(
     "model_name",
     None,
     "Model name from ONNX Hub, for example: resnet50. See"
     " onnx.hub.list_models() to find full list.",
@@ -46,60 +46,66 @@
 )
 
 flags.DEFINE_string(
     "output_dir", None, "Diretory to export the model.", required=True
 )
 
 
-def _download_model(model_name):
+@functools.lru_cache(maxsize=32)
+def _download_model(model_name: str) -> tuple[onnx.ModelProto, hub.ModelInfo]:
   try:
     logging.info("Start downloading model %s", model_name)
     model = hub.load(model_name)
+    model = shape_inference.infer_shapes(model)
+    model_info = hub.get_model_info(model_name)
   except Exception as e:
     raise RuntimeError(f"Fail to download model {model_name}.") from e
 
-  return model
+  return model, model_info
 
 
-def _cosin_sim(a, b):
+def _cosin_sim(a: Any, b: Any) -> float:
   a = np.array(a)
   b = np.array(b)
   a = a.astype(jnp.float32)
   b = b.astype(jnp.float32)
   a = a.flatten()
   b = b.flatten()
   cos_sim = jnp.dot(a, b) / (jnp.linalg.norm(a) * jnp.linalg.norm(b))
   return cos_sim
 
 
-def run_model_from_onnx_backend():
-  """Test standard ONNX Backend API on onnx.hub models."""
+def _get_tensor_type_name(s_type: str) -> str:
+  split_str = s_type.split("(")
+  split_s = split_str[1].split(")")
+  if len(split_s) > 2:
+    raise NotImplementedError("Encountered multiple Tensor types!")
+  return split_s[0]
 
-  model_name_list = list(map(lambda x: x.model.lower(), hub.list_models()))
-  model_name = FLAGS.model_name
-  assert (
-      model_name in model_name_list
-  ), f"{model_name} is valid model name in onnx.hub."
-  model = _download_model(model_name)
+
+def run_model_from_onnx_backend(model_name: str) -> None:
+  """Test standard ONNX Backend API on onnx.hub models."""
+  model, model_info = _download_model(model_name)
 
   try:
     onnx.checker.check_model(model)
   except AttributeError as e:
     logging.warning("Fail to load onnx.checker, skip the check. %s", e)
 
-  model_info = hub.get_model_info(model_name)
   model_info_inputs = list(model_info.metadata.get("io_ports").get("inputs"))
 
   def _create_dummy_tensor(model_info_input):
     shape = model_info_input.get("shape")
     for i, _ in enumerate(shape):
       if isinstance(shape[i], str):
         shape[i] = 1
-      key = jax.random.PRNGKey(0)
-      return jax.random.normal(key, shape)
+    dtype_name = _get_tensor_type_name(model_info_input.get("type"))
+    dtype_value = onnx.TensorProto.DataType.Value(dtype_name.upper())
+    dtype = onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[dtype_value]
+    return np.random.normal(size=shape).astype(dtype)
 
   inputs = [_create_dummy_tensor(item) for item in model_info_inputs]
   results = JaxBackend.run(model, inputs)
   logging.info("jax results shape is = %s", [x.shape for x in results])
 
   try:
     from onnxruntime import backend as OrtBackend  # pylint: disable=g-import-not-at-top
@@ -110,69 +116,66 @@
     print(f"jax and ort similarity = {similarity}")
   except ImportError as e:
     logging.warning(
         "No onnxruntime here. Skip the comparision, err message = %s", e
     )
 
 
-def export_model():
+def export_model(model_name: str, model_path: str) -> None:
   """export jax model to disk."""
   model_name_list = list(map(lambda x: x.model.lower(), hub.list_models()))
-  model_name = FLAGS.model_name
   assert (
       model_name in model_name_list
   ), f"{model_name} is valid model name in onnx.hub."
-  model = _download_model(model_name)
-  model_info = hub.get_model_info(model_name)
+  model, model_info = _download_model(model_name)
   model_info_inputs = list(model_info.metadata.get("io_ports").get("inputs"))
 
   def _create_dummy_tensor(model_info_input):
     shape = model_info_input.get("shape")
     for i, _ in enumerate(shape):
       if isinstance(shape[i], str):
         shape[i] = 1
-      key = jax.random.PRNGKey(0)
-      return jax.random.normal(key, shape, dtype=jnp.float32)
+    key = jax.random.PRNGKey(0)
+    return jax.random.normal(key, shape, dtype=jnp.float32)
 
   inputs = [_create_dummy_tensor(item) for item in model_info_inputs]
   input_names = [item["name"] for item in model_info_inputs]
   dict_inputs = {name: inp for name, inp in zip(input_names, inputs)}
-  jax_model, params = call_onnx.call_onnx(model, inputs)
+  jax_model, params = call_onnx.call_onnx_model(model, inputs)
   output_names = [n.name for n in model.graph.output]
 
   # Wrap the model params and function into a JaxModule.
-  jax_module = JaxModule(
+  jax_module = orbax_export.JaxModule(
       params,
       jax_model,
       trainable=False,
       # input_polymorphic_shape="(b, ...)" if batch_size is None else None,
   )
 
   # Specify the serving configuration and export the model.
   def tf_postprocessor(outputs):
     return {name: output for name, output in zip(output_names, outputs)}
 
   serving_configs = [
-      ServingConfig(
+      orbax_export.ServingConfig(
           signature_key="serving_default",
           input_signature=[
               [
                   tf.TensorSpec(x.shape, x.dtype, name)
                   for x, name in zip(inputs, input_names)
               ]
           ],
           tf_postprocessor=tf_postprocessor,
       ),
   ]
-  em = ExportManager(
+  em = orbax_export.ExportManager(
       jax_module,
       serving_configs,
   )
   # Save the model.
-  model_path = FLAGS.output_dir
   logging.info("Exporting the model to %s.", model_path)
   em.save(model_path)
 
   # Test that the saved model could be loaded and run.
   logging.info("Loading the model from %s.", model_path)
   loaded = tf.saved_model.load(model_path)
 
@@ -185,20 +188,60 @@
       type(savedmodel_output),
       type(jax_output),
   )
   similarity = jax.tree_util.tree_map(_cosin_sim, jax_output, savedmodel_output)
   print(f"jax and savedmodel similarity = {similarity}")
 
 
+def eval_poly_shape(model_name: str) -> None:
+  """Exmaple how to evaluate the polymorphic shape."""
+  model_name_list = list(map(lambda x: x.model.lower(), hub.list_models()))
+  assert (
+      model_name in model_name_list
+  ), f"{model_name} is valid model name in onnx.hub."
+  model, model_info = _download_model(model_name)
+  model_info_inputs = list(model_info.metadata.get("io_ports").get("inputs"))
+
+  def _create_dummy_tensor(model_info_input):
+    shape = model_info_input.get("shape")
+    for i, _ in enumerate(shape):
+      if isinstance(shape[i], str):
+        shape[i] = 1
+    key = jax.random.PRNGKey(0)
+    return jax.random.normal(key, shape, dtype=jnp.float32)
+
+  inputs = [_create_dummy_tensor(item) for item in model_info_inputs]
+  def add_batch_poly_shape(inpt):
+    shape = [str(i) for i in inpt.shape]
+    shape[0] = "batch"
+    return ",".join(shape)
+
+  polymorphic_shapes = jax.tree_map(add_batch_poly_shape, inputs)
+  jax_model, params = call_onnx.call_onnx_model(model, inputs)
+
+  def infer_func(inputs):
+    return jax_model(params, inputs)
+
+  out_spec, out_poly_shape = jax2tf.eval_polymorphic_shape(
+      infer_func, polymorphic_shapes=polymorphic_shapes
+  )(inputs)
+  logging.info("out_spec = %s, out_poly_shape = %s", out_spec, out_poly_shape)
+
+
 def main(argv) -> None:
   if len(argv) > 1:
     raise app.UsageError("Too many command-line arguments.")
+  model_name = FLAGS.model_name
+  model_path = FLAGS.output_dir
+  jax.config.update("jax2tf_default_native_serialization", True)
+  # jax.config.update("jax_enable_x64", True)
+
   logging.info("Start running model from onnx backend.")
-  run_model_from_onnx_backend()
+  run_model_from_onnx_backend(model_name=model_name)
   logging.info("Start exporting model.")
-  jax.config.update("jax2tf_default_native_serialization", True)
-  jax.config.update("jax_enable_x64", True)
-  export_model()
+  export_model(model_name=model_name, model_path=model_path)
+  logging.info("Eval model shape")
+  eval_poly_shape(model_name=model_name)
 
 
 if __name__ == "__main__":
   app.run(main)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/__init__.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/core/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,9 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""JAX based onnxruntime."""
-from .version import __version__
+# Copyright 2023 The Jaxonnxruntime Authors.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/backend.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,38 +8,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Copyright 2023 The Jaxonnxruntime Authors.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """Create the Backend class."""
 # pylint: disable=unused-argument
-
-from typing import Any, NewType
+from typing import Any
 
 import jax
 from jaxonnxruntime import call_onnx
 
 import onnx
 
 
 # Copy from onnx.backend base.py.
 # Due to some reasons, we can not inherit base.py.
 
 
-class DeviceType:
-  """An enumeration of device types."""
-
-  _TYPE = NewType('_TYPE', int)
-  CPU: _TYPE = _TYPE(0)
-  CUDA: _TYPE = _TYPE(1)
-  TPU: _TYPE = _TYPE(2)
-
-
 class BackendRep:
   """Provides an interface for executing an ONNX model on the JAX backend."""
 
   def __init__(self, model: onnx.ModelProto) -> None:
     """Initializes a new instance of the ONNX backend representation class.
 
     Args:
@@ -49,20 +52,20 @@
 
   def run(self, inputs: Any, **kwargs: Any) -> tuple[Any, ...]:
     """Runs the ONNX model using the provided input data.
 
     Args:
       inputs: The input data for the model.
       **kwargs: Additional keyword arguments to pass to the underlying
-        `call_onnx` function.
+        `call_onnx_model` function.
 
     Returns:
       A tuple (Any, ...) of output data produced by the model.
     """
-    model_func, model_params = call_onnx.call_onnx(
+    model_func, model_params = call_onnx.call_onnx_model(
         self._model, inputs, **kwargs
     )
     return model_func(model_params=model_params, inputs=inputs)
 
 
 class Backend:
   """Backend is the entity that will take an ONNX model with inputs.
@@ -84,24 +87,18 @@
       device: The name of the backend device to check for compatibility.
         Defaults to 'CPU'.
 
     Returns:
       True if the model is compatible with the backend device, False otherwise.
     """
     # Check if the specified device is available
-    if device == 'CUDA':
-      try:
-        jax.devices('gpu')
-      except:  # pylint: disable=bare-except
-        return False
-    if device == 'TPU':
-      try:
-        jax.devices('tpu')
-      except:  # pylint: disable=bare-except
-        return False
+    device = device.lower()
+    suppport_devices = [d.platform for d in jax.devices()]
+    if device not in suppport_devices:
+      return False
     return True
 
   @classmethod
   def prepare(
       cls, model: onnx.ModelProto, device: str = 'CPU', **kwargs: Any
   ) -> BackendRep:
     """Prepares an ONNX model for execution on the specified backend device.
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/call_onnx.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/call_onnx.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,139 +8,169 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Copyright 2023 The Jaxonnxruntime Authors.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """Convert ONNX model into jax function."""
 
 import logging
 from typing import Any, Callable, Dict, Sequence, Type, Tuple, Union
 
-from jax import numpy as jnp
-
 from jaxonnxruntime import onnx_ops  # pylint: disable=unused-import
 from jaxonnxruntime.core import handler as onnx_handler
 from jaxonnxruntime.core import onnx_graph
 from jaxonnxruntime.core import onnx_node
+from jaxonnxruntime.core import onnx_utils
 import onnx
 from onnx import defs
-from onnx import numpy_helper
 from onnx.helper import make_opsetid
 
 OnnxNode = onnx_node.OnnxNode
 OnnxGraph = onnx_graph.OnnxGraph
 Handler = onnx_handler.Handler
 
 logger = logging.getLogger(__name__)
 
 
-def call_onnx(
+def call_onnx_model(
     model: onnx.ModelProto, inputs: Union[Sequence[Any], Dict[str, Any]]
 ) -> Tuple[Callable[..., Any], Any]:
-  """Convert. ONNX model to jax_func with model parameters."""
-
-  def _asarray(proto):
-    return jnp.asarray(numpy_helper.to_array(proto).reshape(tuple(proto.dims)))
-
-  tensor_ref_dict = build_ref_dict(model)
+  """Convert ONNX.ModelProto to jax_func with model parameters."""
   graph = model.graph
-  graph_helper = OnnxGraph(graph)
   if model.ir_version < 3:
     opset = [make_opsetid(defs.ONNX_DOMAIN, 1)]
   else:
     opset = model.opset_import
+  model_params = {
+      n.name: onnx_utils.valueinfoproto_asarray(n) for n in graph.initializer
+  }
+  input_names = onnx_utils.get_graph_input(graph)
+  tensor_dict = dict(
+      **onnx_utils.maybe_convert_to_dict(inputs, input_names), **model_params
+  )
+  model_func = call_onnx_graph(graph, tensor_dict, opset=opset)
+  del tensor_dict
+  return model_func, model_params
+
+
+def call_onnx_graph(
+    graph: onnx.GraphProto,
+    tensor_dict: Dict[str, Any],
+    opset: ... = None,
+) -> Callable[..., Any]:
+  """Convert ONNX.GraphProto to jax_func with ONNX.GraphProto.initializer as parameters."""
+  tensor_ref_dict = build_ref_dict(graph)
+  graph_helper = OnnxGraph(graph)
 
   # step 1: Trace those static info
-  model_params = {n.name: _asarray(n) for n in graph.initializer}
   jit_func_dict = {}
   onnx_node_dict = {}
-  opset = [make_opsetid(defs.ONNX_DOMAIN, defs.onnx_opset_version())]
+  opset = (
+    [make_opsetid(defs.ONNX_DOMAIN, defs.onnx_opset_version())]
+    if opset is None
+    else opset
+  )
   handlers = _get_all_handlers(opset)
   node_execute_order_list = graph_helper.topological_sort()
 
-  def _maybe_convert_to_dict(inputs):
-    if isinstance(inputs, dict):
-      return inputs
-    elif isinstance(inputs, Sequence):
-      graph_inputs = graph_helper.get_real_input()
-      assert len(inputs) == len(graph_inputs)
-      return dict(zip(graph_inputs, inputs))
-    else:
-      raise NotImplementedError('Please use inputs of type dict or Sequence!')
-
-  tensor_dict = dict(**_maybe_convert_to_dict(inputs), **model_params)
-
   logger.info('Start tracing the jax_func model to get some static info')
   for node_proto in node_execute_order_list:
     node = OnnxNode(node_proto, graph_helper)
     onnx_node_dict[node.name] = node
     try:
-      node_inputs = [tensor_dict[x] for x in node.inputs]
+      node_inputs = [tensor_dict[x] for x in node.inputs + node.subgraph_inputs]
     except Exception as e:
       raise ValueError(
-          f'failt to get input tensor for node inputs {node.inputs}, the'
-          f' node proto is {node.node_proto}'
+          'Fail to get the input tensor of node input names'
+          f'{node.inputs + node.subgraph_inputs}, the node proto is'
+          f'{node.node_proto}.'
       ) from e
     jit_func = _get_jit_func(node, node_inputs, handlers=handlers)
     jit_func_dict[node.name] = jit_func
     outputs = jit_func(*node_inputs, **node.attrs_dict)
     outputs = outputs if isinstance(outputs, Sequence) else [outputs]
 
     for name, output in zip(node.outputs, outputs):
       tensor_dict[name] = output
-  del tensor_dict
+
+  input_names = onnx_utils.get_graph_input(graph)
 
   def model_func(model_params, inputs):
-    tensor_dict = dict(**_maybe_convert_to_dict(inputs), **model_params)
+    tensor_dict = dict(
+        **onnx_utils.maybe_convert_to_dict(inputs, input_names), **model_params
+    )
     ref_dict = {}
     for node_proto in node_execute_order_list:
       node = onnx_node_dict[node_proto.name]
-      node_inputs = [tensor_dict[x] for x in node.inputs]
+      node_inputs = [tensor_dict[x] for x in node.inputs + node.subgraph_inputs]
       jit_func = jit_func_dict[node.name]
       outputs = jit_func(*node_inputs, **node.attrs_dict)
       outputs = outputs if isinstance(outputs, Sequence) else [outputs]
 
       for name, output in zip(node.outputs, outputs):
         tensor_dict[name] = output
 
-      node_input_shapes = [tensor_dict[x].shape for x in node.inputs]
-      node_output_shapes = [tensor_dict[x].shape for x in node.outputs]
-      logger.debug('\t%s  -> %s', node_input_shapes, node_output_shapes)
+      # Below lines may cause error when tensor_dict[x] is a list
+      # Comment out because they are only for debugging
+      # node_input_shapes = [tensor_dict[x].shape for x in node.inputs]
+      # node_output_shapes = [tensor_dict[x].shape for x in node.outputs]
+      # logger.debug('\t%s  -> %s', node_input_shapes, node_output_shapes)
 
-      for input_ in node.inputs:
+      for input_ in node.inputs + node.subgraph_inputs:
         if input_ in ref_dict:
           ref_dict[input_] += 1
         else:
           ref_dict[input_] = 1
       remove_keys = []
       for k, v in ref_dict.items():
         if tensor_ref_dict[k] == v:
           remove_keys.append(k)
       for rm_k in remove_keys:
         del ref_dict[rm_k]
         del tensor_dict[rm_k]
 
     return [tensor_dict[n.name] for n in graph.output]
 
-  return model_func, model_params
+  return model_func
 
 
-def build_ref_dict(model: onnx.ModelProto) -> Dict[str, int]:
+def build_ref_dict(graph: onnx.GraphProto) -> Dict[str, int]:
   """Initialize reference count dict."""
   ref_dict: dict[Any, Any] = {}
-  for node in model.graph.node:
+  for node in graph.node:
+    if onnx_utils.contain_subgraph(node):
+      for a in node.attribute:
+        if a.HasField('g'):
+          sub_ref_dict = build_ref_dict(a.g)
+          ref_dict.update(
+              {k: ref_dict.get(k, 0) + v for k, v in sub_ref_dict.items()}
+          )
     inputs = node.input
     for input_ in inputs:
       if input_ in ref_dict:
         ref_dict[input_] += 1
       else:
         ref_dict[input_] = 1
-
+  for o in graph.output:
+    ref_dict[o.name] = ref_dict[o.name] + 1 if o.name in ref_dict else 1
   return ref_dict
 
 
 def _get_all_handlers(
     opset: Sequence[onnx.OperatorSetIdProto],
 ) -> Dict[str, Dict[str, Type[Handler]]]:
   """Get all ONNX OP_TYPE handlers from Handler subclasses.
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/core/handler.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/core/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Copyright 2023 The Jaxonnxruntime Authors.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """Defines a Handler class and a decorator to register ONNX ops."""
 import logging
 
 from typing import Any, Sequence
 from onnx import defs
 
 logger = logging.getLogger(__name__)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/core/onnx_graph.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/core/onnx_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Copyright 2023 The Jaxonnxruntime Authors.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """Wrap the onnx.GraphProto as OnnxGraph class and provide useful graph manipulation methods."""
+import collections
 from typing import Any, List, Sequence
+
 import onnx
 
 
 class OnnxGraph:
   """Graph class wrapper of ONNX.GraphProto.
 
   Attributes:
@@ -136,25 +151,35 @@
     for output_ in outputs:
       if output_ in tensor_down_to_node_dict:
         results.extend(tensor_down_to_node_dict[output_])
     return results
 
   def topological_sort(self) -> Sequence[onnx.NodeProto]:
     """Return the topological sort order of those nodes."""
+    in_degree = collections.defaultdict(int)
+    for u in self.node_dict:
+      if u not in in_degree:
+        in_degree[u] = 0
+      for v in self.get_child_nodes_name(u):
+        in_degree[v] += 1
+
+    queue = collections.deque(
+        [v for v in in_degree.keys() if in_degree[v] == 0]
+    )
+    sorted_list = []
+
+    while queue:
+      u = queue.popleft()
+      sorted_list.append(u)
+
+      for v in self.get_child_nodes_name(u):
+        in_degree[v] -= 1
+        if in_degree[v] == 0:
+          queue.append(v)
+
+    if len(sorted_list) != len(self.node_dict):
+      raise RuntimeError(
+          f"Graph has a cycle, sorted_list={sorted_list},"
+          f" node_dict={self.node_dict.keys()}"
+      )
 
-    visited = {}
-    stack = []
-
-    # A recursive function used by topologicalSort
-    def topological_sort_util(v):
-      visited[v] = True
-      for i in self.get_child_nodes_name(v):
-        if i not in visited or not visited[i]:
-          topological_sort_util(i)
-      stack.append(v)
-
-    for i in self.node_dict:
-      if i not in visited or not visited[i]:
-        topological_sort_util(i)
-
-    # return list in reverse order.
-    return list(reversed([self.node_dict[n] for n in stack]))
+    return [self.node_dict[n] for n in sorted_list]
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/abs.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/abs.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,22 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 Abs op."""
+    cls._prepare(node, inputs, onnx_abs)
+    return onnx_abs
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 Abs op."""
     cls._prepare(node, inputs, onnx_abs)
     return onnx_abs
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/add.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,22 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_7(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_7 Add op."""
+    cls._prepare(node, inputs, onnx_add)
+    return onnx_add
+
+  @classmethod
   def version_14(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_14 Add op."""
     cls._prepare(node, inputs, onnx_add)
     return onnx_add
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/averagepool.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/neg.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,92 +21,52 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX AveragePool operator."""
+"""Define ONNX Neg operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
-from typing import Any, Union
+import inspect
+from typing import Any
 
 from jax import jit
-from jax import lax
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
-import numpy as np
 
-from .maxpool import MaxPool
 
-
-@handler.register_op("AveragePool")
-class AveragePool(handler.Handler):
-  """Implementation of the ONNX AveragePool operator."""
+@handler.register_op("Neg")
+class Neg(handler.Handler):
+  """Implementation of the ONNX Neg operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    MaxPool._prepare(node, inputs, onnx_jax_impl)  # pylint: disable=protected-access
-    node.attrs_dict["count_include_pad"] = node.attrs.get(
-        "count_include_pad", 0
-    )
-    del node.attrs_dict["storage_order"]
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_11(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_11 AveragePool op."""
-    cls._prepare(node, inputs, onnx_averagepool)
-    return onnx_averagepool
-
-
-@functools.partial(
-    jit,
-    static_argnames=(
-        "ceil_mode",
-        "strides",
-        "pads",
-        "dilations",
-        "kernel_shape",
-        "count_include_pad",
-    ),
-)
-def onnx_averagepool(
-    *input_args,
-    ceil_mode: int,
-    strides: Sequence[int],
-    pads: Union[Sequence[tuple[int, int]], str],
-    dilations: Sequence[int],
-    kernel_shape: Sequence[int],
-    count_include_pad: int,
-):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#MaxPool for more details."""
+    """ONNX version_13 Neg op."""
+    cls._prepare(node, inputs, onnx_neg)
+    return onnx_neg
+
+
+@functools.partial(jit, static_argnames=())
+def onnx_neg(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Neg for more details."""
   assert len(input_args) == 1
-  x = input_args[0]
-  if ceil_mode != 0:
-    raise ValueError("ceil_mode = 1 is not implement yet.")
-
-  if count_include_pad == 0:
-    one = jnp.ones_like(x, dtype=x.dtype)
-    wsizes = lax.reduce_window(one, 0.0, lax.add, kernel_shape, strides, pads)
-  else:
-    wsizes = np.prod(kernel_shape)
-
-  return (
-      lax.reduce_window(
-          x,
-          jnp.array(0, dtype=x.dtype),
-          lax.add,
-          kernel_shape,
-          strides,
-          pads,
-          None,
-          dilations,
-      )
-      / wsizes
-  )
+  return jnp.negative(input_args[0])
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/batchnormalization.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/equal.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,63 +21,60 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX BatchNormalization operator."""
+"""Define ONNX Equal operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
+import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('BatchNormalization')
-class BatchNormalization(handler.Handler):
-  """Implementation of the ONNX BatchNormalization operator."""
+@handler.register_op("Equal")
+class Equal(handler.Handler):
+  """Implementation of the ONNX Equal operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    node.attrs_dict['epsilon'] = node.attrs.get('epsilon', 1e-5)
-    node.attrs_dict['momentum'] = node.attrs.get('momentum', 0.9)
-    node.attrs_dict['training_mode'] = node.attrs.get('training_mode', 0)
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_15(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_15 BatchNormalization op."""
-    cls._prepare(node, inputs, onnx_batchnormalization)
-    return onnx_batchnormalization
-
-
-@functools.partial(
-    jit, static_argnames=('epsilon', 'momentum', 'training_mode')
-)
-def onnx_batchnormalization(
-    *input_args, epsilon: float, momentum: float, training_mode: int
-):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#BatchNormalization for more details."""
-  x, scale, b, input_mean, input_var = input_args
-
-  dims_x = len(x.shape)
-  dim_ones = (1,) * (dims_x - 2)
-  scale = scale.reshape(-1, *dim_ones)
-  b = b.reshape(-1, *dim_ones)
-  input_mean = input_mean.reshape(-1, *dim_ones)
-  input_var = input_var.reshape(-1, *dim_ones)
-
-  if training_mode == 0:
-    return (x - input_mean) / jnp.sqrt(input_var + epsilon) * scale + b
-  else:
-    raise NotImplementedError(
-        'BatchNormalization with training_mode was not implemented yet.'
-    )
+    """ONNX version_13 Equal op."""
+    cls._prepare(node, inputs, onnx_equal)
+    return onnx_equal
+
+  @classmethod
+  def version_19(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_19 Equal op."""
+    cls._prepare(node, inputs, onnx_equal)
+    return onnx_equal
+
+
+@functools.partial(jit, static_argnames=())
+def onnx_equal(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Equal for more details."""
+  assert len(input_args) == 2
+  return jnp.equal(input_args[0], input_args[1])
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/cast.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/transpose.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,75 +21,59 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Cast operator."""
+"""Define ONNX Transpose operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
+
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
-import onnx
-
-register_op = handler.register_op
-Handler = handler.Handler
-OnnxNode = onnx_node.OnnxNode
 
 
-@handler.register_op("Cast")
-class Cast(handler.Handler):
-  """Implementation of the ONNX Cast operator."""
+@handler.register_op("Transpose")
+class Transpose(handler.Handler):
+  """Implementation of the ONNX Transpose operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
         param.name
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
-    if not node.attrs_dict["from_type"]:
-      from_type = node.context_graph.value_info_dict[
-          node.inputs[0]
-      ].type.tensor_type.elem_type
-      node.attrs_dict["from_type"] = from_type
+
+  @classmethod
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 Transpose op."""
+    cls._prepare(node, inputs, onnx_transpose)
+    return onnx_transpose
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Cast op."""
-    cls._prepare(node, inputs, onnx_cast)
-    return onnx_cast
-
-
-@functools.partial(jit, static_argnames=("to", "from_type"))
-def onnx_cast(x, *, to, from_type=None):
-  if from_type is onnx.TensorProto.STRING or to is onnx.TensorProto.STRING:
-    raise NotImplementedError(
-        "Cast JAX version do not support STRING type yet."
-    )
-  to_type = tensor_dtype_to_jnp_dtype(to)
-  from_type = tensor_dtype_to_jnp_dtype(from_type) if from_type else x.dtype
-  try:
-    return x.view(from_type).astype(to_type)
-  except Exception as e:
-    raise ValueError(
-        f"onnx_cast can not support from_type = {from_type}, to_type ="
-        f" {to_type}"
-    ) from e
-
-
-def tensor_dtype_to_jnp_dtype(tensor_type):
-  if tensor_type is onnx.TensorProto.BFLOAT16:
-    return jnp.bfloat16
-  return jnp.dtype(onnx.helper.mapping.TENSOR_TYPE_TO_NP_TYPE[tensor_type])
+    """ONNX version_13 Transpose op."""
+    cls._prepare(node, inputs, onnx_transpose)
+    return onnx_transpose
+
+
+@functools.partial(jit, static_argnames="perm")
+def onnx_transpose(*input_args, perm):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Transpose."""
+  assert len(input_args) == 1
+  x = input_args[0]
+  return jnp.transpose(x, perm)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/concat.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/exp.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Concat operator."""
+"""Define ONNX Exp operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Concat")
-class Concat(handler.Handler):
-  """Implementation of the ONNX Concat operator."""
+@handler.register_op("Exp")
+class Exp(handler.Handler):
+  """Implementation of the ONNX Exp operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -54,16 +54,18 @@
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Concat op."""
-    cls._prepare(node, inputs, onnx_concat)
-    return onnx_concat
+    """ONNX version_13 Exp op."""
+    cls._prepare(node, inputs, onnx_exp)
+    return onnx_exp
 
 
-@functools.partial(jit, static_argnames="axis")
-def onnx_concat(*input_args, axis=0):
-  """The internal jax impl for onnx Concat op."""
-  return jnp.concatenate(input_args, axis=axis)
+@functools.partial(jit, static_argnames=())
+def onnx_exp(*input_args):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Exp."""
+  assert len(input_args) == 1
+  x = input_args[0]
+  return jnp.exp(x)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/constant.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,20 +78,36 @@
         matched = matched + 1
 
     assert (
         matched == 1
     ), f'Should only provide one of value attributes, but get {matched}'
 
   @classmethod
+  def version_9(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_9 Constant op."""
+    cls._prepare(node, inputs, onnx_constant)
+    return onnx_constant
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 Constant op."""
     cls._prepare(node, inputs, onnx_constant)
     return onnx_constant
 
+  @classmethod
+  def version_19(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_19 Constant op."""
+    cls._prepare(node, inputs, onnx_constant)
+    return onnx_constant
+
 
 @functools.partial(jit, static_argnames=())
 def onnx_constant(*input_args, value):
   """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Constant."""
   assert len(input_args) == 0
   return value
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/constantofshape.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/constantofshape.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/conv.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,22 @@
       }
       assert (
           pad_str_type in onnx_to_jax_pad_type
       ), f"Invalid auto_pad attribute: {pad_str_type}"
       node.attrs_dict["pads"] = onnx_to_jax_pad_type[pad_str_type]
 
   @classmethod
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 Conv op."""
+    cls._prepare(node, inputs, onnx_conv)
+    return onnx_conv
+
+  @classmethod
   def version_11(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_11 Conv op."""
     cls._prepare(node, inputs, onnx_conv)
     return onnx_conv
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/div.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/or_op.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Div operator."""
+"""Define ONNX Or operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Div")
-class Div(handler.Handler):
-  """Implementation of the ONNX Div operator."""
+@handler.register_op("Or")
+class Or(handler.Handler):
+  """Implementation of the ONNX Or operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,26 +53,20 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_14(
+  def version_7(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_14 Div op."""
-    cls._prepare(node, inputs, onnx_div)
-    return onnx_div
+    """ONNX version_7 Or op."""
+    cls._prepare(node, inputs, onnx_or)
+    return onnx_or
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_div(*input_args):
-  """The internal jax impl for onnx Div op."""
+def onnx_or(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Or for more details."""
   assert len(input_args) == 2
-  x, y = input_args
-  if jnp.issubdtype(x.dtype, jnp.integer) and jnp.issubdtype(
-      y.dtype, jnp.integer
-  ):
-    return jnp.floor_divide(x, y)
-  else:
-    return jnp.true_divide(x, y)
+  return jnp.logical_or(input_args[0], input_args[1])
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/exp.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/tanh.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Exp operator."""
+"""Define ONNX Tanh operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Exp")
-class Exp(handler.Handler):
-  """Implementation of the ONNX Exp operator."""
+@handler.register_op("Tanh")
+class Tanh(handler.Handler):
+  """Implementation of the ONNX Tanh operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,21 +51,29 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 Tanh op."""
+    cls._prepare(node, inputs, onnx_tanh)
+    return onnx_tanh
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Exp op."""
-    cls._prepare(node, inputs, onnx_exp)
-    return onnx_exp
+    """ONNX version_13 Tanh op."""
+    cls._prepare(node, inputs, onnx_tanh)
+    return onnx_tanh
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_exp(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Exp."""
+def onnx_tanh(*input_args):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Tanh."""
   assert len(input_args) == 1
   x = input_args[0]
-  return jnp.exp(x)
+  return jnp.tanh(x)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/flatten.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/ceil.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Flatten operator."""
+"""Define ONNX Ceil operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
+
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
-import numpy as np
 
 
-@handler.register_op("Flatten")
-class Flatten(handler.Handler):
-  """Implementation of the ONNX Flatten operator."""
+@handler.register_op("Ceil")
+class Ceil(handler.Handler):
+  """Implementation of the ONNX Ceil operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -56,24 +56,17 @@
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Flatten op."""
-    cls._prepare(node, inputs, onnx_flatten)
-    return onnx_flatten
+    """ONNX version_13 Ceil op."""
+    cls._prepare(node, inputs, onnx_ceil)
+    return onnx_ceil
 
 
-@functools.partial(jit, static_argnames="axis")
-def onnx_flatten(*input_args, axis):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Flatten for more details."""
-  axis = 1 if axis is None else axis
+@functools.partial(jit, static_argnames=())
+def onnx_ceil(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Ceil for more details."""
   assert len(input_args) == 1
-  x = input_args[0]
-  dim = len(x.shape)
-  assert axis < dim and axis >= -dim, f"axis should with [{-dim}, {dim}]"
-  new_shape = (
-      (1, -1) if axis == 0 else (np.prod(x.shape[0:axis]).astype(int), -1)
-  )
-  return jnp.reshape(x, new_shape)
+  return jnp.ceil(input_args[0])
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/gather.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/gather.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,30 @@
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     node.attrs_dict["axis"] = node.attrs.get("axis", 0)
 
   @classmethod
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 Gather op."""
+    cls._prepare(node, inputs, onnx_gather)
+    return onnx_gather
+
+  @classmethod
+  def version_11(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_11 Gather op."""
+    cls._prepare(node, inputs, onnx_gather)
+    return onnx_gather
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 Gather op."""
     cls._prepare(node, inputs, onnx_gather)
     return onnx_gather
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/gemm.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/gemm.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,14 +51,30 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_7(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_7 Gemm op."""
+    cls._prepare(node, inputs, onnx_gemm)
+    return onnx_gemm
+
+  @classmethod
+  def version_9(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_9 Gemm op."""
+    cls._prepare(node, inputs, onnx_gemm)
+    return onnx_gemm
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 Gemm op."""
     cls._prepare(node, inputs, onnx_gemm)
     return onnx_gemm
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/globalaveragepool.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/globalaveragepool.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/leakyrelu.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/leakyrelu.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/matmul.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/matmul.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,22 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_9(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_9 MatMul op."""
+    cls._prepare(node, inputs, onnx_matmul)
+    return onnx_matmul
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 MatMul op."""
     cls._prepare(node, inputs, onnx_matmul)
     return onnx_matmul
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/maxpool.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/maxpool.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,14 +101,22 @@
       }
       assert (
           pad_str_type in onnx_to_jax_pad_type
       ), f"Invalid auto_pad attribute: {pad_str_type}"
       node.attrs_dict["pads"] = onnx_to_jax_pad_type[pad_str_type]
 
   @classmethod
+  def version_8(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_8 MaxPool op."""
+    cls._prepare(node, inputs, onnx_maxpool)
+    return onnx_maxpool
+
+  @classmethod
   def version_12(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_12 MaxPool op."""
     cls._prepare(node, inputs, onnx_maxpool)
     return onnx_maxpool
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/mul.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/mul.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,14 +51,22 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_7(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_7 Mul op."""
+    cls._prepare(node, inputs, onnx_mul)
+    return onnx_mul
+
+  @classmethod
   def version_14(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_14 Mul op."""
     cls._prepare(node, inputs, onnx_mul)
     return onnx_mul
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/nonzero.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/max.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,51 +21,56 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX NonZero operator."""
+"""Define ONNX Max operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
+import functools
 import inspect
-import logging
 from typing import Any
 
+from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("NonZero")
-class NonZero(handler.Handler):
-  """Implementation of the ONNX NonZero operator."""
+@handler.register_op("Max")
+class Max(handler.Handler):
+  """Implementation of the ONNX Max operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
         param.name
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
+    node.attrs_dict["arg_num"] = len(node.inputs)
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 NonZero op."""
-    cls._prepare(node, inputs, onnx_nonzero)
-    return onnx_nonzero
+    """ONNX version_13 Max op."""
+    cls._prepare(node, inputs, onnx_max)
+    return onnx_max
 
 
-# @functools.partial(jit, static_argnames=("size"))
-def onnx_nonzero(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#NonZero."""
-  assert len(input_args) == 1
-  logging.warning("onnx_nonzero cann not support jax.jit mode.")
-  (x,) = input_args
-  return jnp.stack(jnp.nonzero(x))
+@functools.partial(jit, static_argnames=("arg_num",))
+def onnx_max(*input_args, arg_num):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Max for more details."""
+  assert len(input_args) == arg_num
+  res = input_args[0]
+  for i in range(arg_num):
+    res = jnp.maximum(res, input_args[i])
+  return res
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/pad.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/range.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,62 +21,55 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Pad operator."""
+"""Define ONNX Range operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
+from jaxonnxruntime import config
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Pad')
-class Pad(handler.Handler):
-  """Implementation of the ONNX Pad operator."""
+@handler.register_op("Range")
+class Range(handler.Handler):
+  """Implementation of the ONNX Range operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    node.attrs_dict['mode'] = node.attrs.get('mode', 'constant')
-    node.attrs_dict['pads'] = tuple(inputs[1].tolist())
-
-    if len(inputs) >= 3:
-      node.attrs_dict['constant_value'] = inputs[2].item()
-    else:
-      node.attrs_dict['constant_value'] = 0.0
+    if config.jaxort_only_allow_initializers_as_static_args:
+      for inp in node.inputs[1:]:
+        if inp not in node.context_graph.initializer_dict:
+          raise ValueError(
+              f"{inp} is not constant but used as a static argument "
+              "when `jax.jit` the `Range` operator. "
+              "The jitted function gives wrong results if its value changes."
+          )
+    node.attrs_dict["start"] = inputs[0].item()
+    node.attrs_dict["limit"] = inputs[1].item()
+    node.attrs_dict["delta"] = inputs[2].item()
+    node.attrs_dict["dtype"] = inputs[0].dtype
 
   @classmethod
-  def version_13(
+  def version_11(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Pad op."""
-    cls._prepare(node, inputs, onnx_pad)
-    return onnx_pad
-
-
-@functools.partial(jit, static_argnames=('pads', 'constant_value', 'mode'))
-def onnx_pad(*input_args, pads, constant_value=0.0, mode='constant'):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Pad."""
-  x = input_args[0]
-  input_rank = x.ndim
-  if input_rank * 2 != jnp.size(pads):
-    raise ValueError(
-        'The number of elements in raw_pads should be 2 * input_rank'
-        f'pads = {pads}, input_rank = {input_rank}'
-    )
-
-  # re-order to np.pad accepted order ((x1_begin, x1_end), (x2_begin, x2_end))
-  pad_width = ()
-  for i in range(int(jnp.size(pads) / 2)):
-    pad_width += (((pads[i], pads[i + input_rank])),)
-
-  if mode == 'constant':
-    return jnp.pad(x, pad_width, mode, constant_values=constant_value)
-  return jnp.pad(x, pad_width, mode)
+    """ONNX version_11 Range op."""
+    cls._prepare(node, inputs, onnx_range)
+    return onnx_range
+
+
+@functools.partial(jit, static_argnames=("start", "limit", "delta", "dtype"))
+def onnx_range(*_, start, limit, delta, dtype):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Range for more details."""
+  return jnp.arange(start, stop=limit, step=delta, dtype=dtype)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/pow.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/pow.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,30 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_7(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_7 Pow op."""
+    cls._prepare(node, inputs, onnx_pow)
+    return onnx_pow
+
+  @classmethod
+  def version_12(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_12 Pow op."""
+    cls._prepare(node, inputs, onnx_pow)
+    return onnx_pow
+
+  @classmethod
   def version_15(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_15 Pow op."""
     cls._prepare(node, inputs, onnx_pow)
     return onnx_pow
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/reducemax.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/less.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,54 +21,52 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX ReduceMax operator."""
+"""Define ONNX Less operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('ReduceMax')
-class ReduceMax(handler.Handler):
-  """Implementation of the ONNX ReduceMax operator."""
+@handler.register_op("Less")
+class Less(handler.Handler):
+  """Implementation of the ONNX Less operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
         param.name
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
-    node.attrs_dict['keepdims'] = (
-        True if node.attrs_dict['keepdims'] == 1 else False
-    )
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 ReduceMax op."""
-    cls._prepare(node, inputs, onnx_reducemax)
-    return onnx_reducemax
+    """ONNX version_13 Less op."""
+    cls._prepare(node, inputs, onnx_less)
+    return onnx_less
 
 
-@functools.partial(jit, static_argnames=('axes', 'keepdims'))
-def onnx_reducemax(*input_args, axes, keepdims=True):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#ReduceMax."""
-  assert len(input_args) == 1
-  x = input_args[0]
-  return jnp.max(x, axis=axes, keepdims=keepdims)
+@functools.partial(jit, static_argnames=())
+def onnx_less(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Less for more details."""
+  assert len(input_args) == 2
+  return jnp.less(input_args[0], input_args[1])
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/reducemean.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reciprocal.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,52 +21,60 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX ReduceMean operator."""
+"""Define ONNX Reciprocal operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('ReduceMean')
-class ReduceMean(handler.Handler):
-  """Implementation of the ONNX ReduceMean operator."""
+@handler.register_op("Reciprocal")
+class Reciprocal(handler.Handler):
+  """Implementation of the ONNX Reciprocal operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
         param.name
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
-    node.attrs_dict['keepdims'] = node.attrs.get('keepdims', True)
+
+  @classmethod
+  def version_6(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_6 Reciprocal op."""
+    cls._prepare(node, inputs, onnx_reciprocal)
+    return onnx_reciprocal
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 ReduceMean op."""
-    cls._prepare(node, inputs, onnx_reducemean)
-    return onnx_reducemean
+    """ONNX version_13 Reciprocal op."""
+    cls._prepare(node, inputs, onnx_reciprocal)
+    return onnx_reciprocal
 
 
-@functools.partial(jit, static_argnames=('axes', 'keepdims'))
-def onnx_reducemean(*input_args, axes=None, keepdims=True):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#ReduceMean."""
+@functools.partial(jit, static_argnames=())
+def onnx_reciprocal(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Reciprocal for more details."""
   assert len(input_args) == 1
-  data = input_args[0]
-  return jnp.mean(data, axis=axes, keepdims=keepdims)
+  return jnp.reciprocal(input_args[0])
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/reducesum.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reducesum.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Define ONNX ReduceSum operator."""
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
+import functools
 import inspect
 from typing import Any
-
+from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
 @handler.register_op('ReduceSum')
 class ReduceSum(handler.Handler):
@@ -67,15 +68,17 @@
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 ReduceSum op."""
     cls._prepare(node, inputs, onnx_reducesum)
     return onnx_reducesum
 
 
-# @functools.partial(jit, static_argnames=('axes', 'keepdims'))
+@functools.partial(
+    jit, static_argnames=('axes', 'keepdims', 'noop_with_empty_axes')
+)
 def onnx_reducesum(
     *input_args, axes=None, keepdims=False, noop_with_empty_axes=None
 ):
   """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#ReduceSum."""
   assert len(input_args) == 1 or len(input_args) == 2
   data = input_args[0]
   noop_with_empty_axes = 0 if not noop_with_empty_axes else noop_with_empty_axes
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/relu.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sigmoid.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Relu operator."""
+"""Define ONNX Sigmoid operator."""
 # pylint: disable=unused-argument
 # pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 import jax
 from jax import jit
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Relu")
-class Relu(handler.Handler):
-  """Implementation of the ONNX Relu operator."""
+@handler.register_op("Sigmoid")
+class Sigmoid(handler.Handler):
+  """Implementation of the ONNX Sigmoid operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -53,21 +53,20 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_14(
+  def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_14 Relu op."""
-    cls._prepare(node, inputs, onnx_relu)
-    return onnx_relu
+    """ONNX version_13 Sigmoid op."""
+    cls._prepare(node, inputs, onnx_sigmoid)
+    return onnx_sigmoid
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_relu(*input_args):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Relu for more details."""
+def onnx_sigmoid(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sigmoid for more details."""
   assert len(input_args) == 1
-  x = input_args[0]
-  return jax.nn.relu(x)
+  return jax.nn.sigmoid(input_args[0])
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/reshape.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/reshape.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,38 +27,63 @@
 # limitations under the License.
 """Define ONNX Reshape operator."""
 from collections.abc import Callable, Sequence
 import functools
 from typing import Any
 from jax import jit
 from jax import numpy as jnp
+from jaxonnxruntime import config
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 import numpy as np
 
 
 @handler.register_op('Reshape')
 class Reshape(handler.Handler):
   """Implementation of the ONNX Reshape operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
+    if config.jaxort_only_allow_initializers_as_static_args:
+      if node.inputs[1] not in node.context_graph.initializer_dict:
+        raise ValueError(
+            f'{node.inputs[1]} is not constant but used as `shape` of Reshape'
+            ' static argument during `jax.jit`. '
+            'the jitted function gives wrong results if its value changes '
+            'in another input.'
+        )
     node.attrs_dict['shape'] = tuple(inputs[1].tolist())
     node.attrs_dict['allowzero'] = node.attrs.get('allowzero', 0)
 
   @classmethod
+  def version_5(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_5 Reshape op."""
+    cls._prepare(node, inputs, onnx_reshape)
+    return onnx_reshape
+
+  @classmethod
   def version_14(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_14 Reshape op."""
     cls._prepare(node, inputs, onnx_reshape)
     return onnx_reshape
 
+  @classmethod
+  def version_19(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_19 Reshape op."""
+    cls._prepare(node, inputs, onnx_reshape)
+    return onnx_reshape
+
 
 @functools.partial(jit, static_argnames=('shape', 'allowzero'))
 def onnx_reshape(*input_args, shape, allowzero):
   """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Reshape."""
   assert len(input_args) == 2
   data, _ = input_args
   new_shape = np.copy(shape)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/shape.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sqrt.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Shape operator."""
+"""Define ONNX Sqrt operator."""
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Shape')
-class Shape(handler.Handler):
-  """Implementation of the ONNX Shape operator."""
+@handler.register_op("Sqrt")
+class Sqrt(handler.Handler):
+  """Implementation of the ONNX Sqrt operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,22 +51,28 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_15(
+  def version_6(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_15 Shape op."""
-    cls._prepare(node, inputs, onnx_shape)
-    return onnx_shape
+    """ONNX version_6 Sqrt op."""
+    cls._prepare(node, inputs, onnx_sqrt)
+    return onnx_sqrt
+
+  @classmethod
+  def version_13(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_13 Sqrt op."""
+    cls._prepare(node, inputs, onnx_sqrt)
+    return onnx_sqrt
 
 
-@functools.partial(jit, static_argnames=('start', 'end'))
-def onnx_shape(*input_args, start=None, end=None):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Shape."""
+@functools.partial(jit, static_argnames=())
+def onnx_sqrt(*input_args):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sqrt."""
   assert len(input_args) == 1
-  x = input_args[0]
-  dims = x.shape[start:end]
-  return jnp.asarray(dims)
+  return jnp.sqrt(*input_args)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/slice.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/split.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,58 +21,86 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Slice operator."""
+"""Define ONNX Split operator."""
 from collections.abc import Callable, Sequence
+import functools
 from typing import Any
 
+from jax import jit
+from jax import lax
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Slice')
-class Slice(handler.Handler):
-  """Implementation of the ONNX Slice operator."""
+@handler.register_op('Split')
+class Split(handler.Handler):
+  """Implementation of the ONNX Split operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    node.attrs_dict['starts'] = tuple(inputs[1].tolist())
-    node.attrs_dict['ends'] = tuple(inputs[2].tolist())
-    if len(inputs) >= 4:
-      node.attrs_dict['axes'] = tuple(inputs[3].tolist())
-    else:
-      node.attrs_dict['axes'] = None
-    if len(inputs) >= 5:
-      node.attrs_dict['steps'] = tuple(inputs[4].tolist())
-    else:
-      node.attrs_dict['steps'] = None
+    node.attrs_dict['axis'] = (
+        0 if 'axis' not in node.attrs else node.attrs['axis']
+    )
+    node.attrs_dict['num_output'] = node.len_outputs
+    if len(inputs) >= 2:
+      node.attrs_dict['split'] = tuple(inputs[1].tolist())
+
+  @classmethod
+  def version_2(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_2 Split op."""
+    cls._prepare(node, inputs, onnx_split)
+    return onnx_split
+
+  @classmethod
+  def version_11(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_11 Split op."""
+    cls._prepare(node, inputs, onnx_split)
+    return onnx_split
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Slice op."""
-    cls._prepare(node, inputs, onnx_slice)
-    return onnx_slice
+    """ONNX version_13 Split op."""
+    cls._prepare(node, inputs, onnx_split)
+    return onnx_split
 
+  @classmethod
+  def version_18(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_18 Split op."""
+    cls._prepare(node, inputs, onnx_split)
+    return onnx_split
+
+
+@functools.partial(jit, static_argnames=('split', 'axis', 'num_output'))
+def onnx_split(*input_args, num_output, split=None, axis=0):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Split for more details."""
 
-# @functools.partial(jit, static_argnames=('starts', 'ends', 'axes', 'steps'))
-def onnx_slice(*input_args, starts, ends, axes, steps):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Slice."""
   x = input_args[0]
-  if axes is None:
-    axes = tuple(range(len(starts)))
-  if steps is None:
-    steps = [1] * len(starts)
-  slices = tuple(
-      slice(start, end, step) for start, end, step in zip(starts, ends, steps)
-  )
-  sub_indx = [slice(None)] * len(x.shape)
-  for i, axis in enumerate(axes):
-    sub_indx[axis] = slices[i]
-  return x[tuple(sub_indx)]
+  if split is None:
+    split = [x.shape[axis] // num_output] * num_output
+  starts = []
+  ends = []
+  starts.append([0] * x.ndim)
+  for idx in range(1, num_output):
+    st = [0] * x.ndim
+    st[axis] = sum(split[:idx])
+    starts.append(st)
+    en = list(x.shape)
+    en[axis] = sum(split[:idx])
+    ends.append(en)
+  ends.append(list(x.shape))
+
+  return [lax.slice(x, start, end) for start, end in zip(starts, ends)]
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/softmax.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/where.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,41 +21,53 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Softmax operator."""
+"""Define ONNX Where operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
+import functools
+import inspect
 from typing import Any
 
-import jax
+from jax import jit
+from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Softmax')
-class Softmax(handler.Handler):
-  """Implementation of the ONNX Softmax operator."""
+@handler.register_op("Where")
+class Where(handler.Handler):
+  """Implementation of the ONNX Where operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    node.attrs_dict['axis'] = node.attrs.get('axis', -1)
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_13(
+  def version_16(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Softmax op."""
-    cls._prepare(node, inputs, onnx_softmax)
-    return onnx_softmax
+    """ONNX version_16 Where op."""
+    cls._prepare(node, inputs, onnx_where)
+    return onnx_where
 
 
-# @functools.partial(jit, static_argnames=('axis'))
-def onnx_softmax(*input_args, axis):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Softmax."""
-  assert len(input_args) == 1
-  x = input_args[0]
-  return jax.nn.softmax(x, axis=axis)
+@functools.partial(jit, static_argnames=())
+def onnx_where(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Where for more details."""
+  assert len(input_args) == 3
+  cond, x, y = input_args
+  return jnp.where(cond, x, y)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/split.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/expand.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,62 +21,60 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Split operator."""
+"""Define ONNX Expand operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 from typing import Any
 
 from jax import jit
-from jax import lax
+from jax import numpy as jnp
+from jaxonnxruntime import config
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Split')
-class Split(handler.Handler):
-  """Implementation of the ONNX Split operator."""
+@handler.register_op("Expand")
+class Expand(handler.Handler):
+  """Implementation of the ONNX Expand operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    node.attrs_dict['axis'] = (
-        0 if 'axis' not in node.attrs else node.attrs['axis']
-    )
-    node.attrs_dict['num_output'] = node.len_outputs
-    if len(inputs) >= 2:
-      node.attrs_dict['split'] = tuple(inputs[1].tolist())
+    if config.jaxort_only_allow_initializers_as_static_args:
+      if node.inputs[1] not in node.context_graph.initializer_dict:
+        raise ValueError(
+            f"{node.inputs[1]} is not constant but used as a static argument "
+            "`shape` when `jax.jit` the `Expand` operator. "
+            "The jitted function gives wrong results if its value changes."
+        )
+    node.attrs_dict["shape"] = tuple(inputs[1].tolist())
+
+  @classmethod
+  def version_8(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_8 Expand op."""
+    cls._prepare(node, inputs, onnx_expand)
+    return onnx_expand
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Split op."""
-    cls._prepare(node, inputs, onnx_split)
-    return onnx_split
-
-
-@functools.partial(jit, static_argnames=('split', 'axis', 'num_output'))
-def onnx_split(*input_args, num_output, split=None, axis=0):
-  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Split for more details."""
-
-  x = input_args[0]
-  if split is None:
-    split = [x.shape[axis] // num_output] * num_output
-  starts = []
-  ends = []
-  starts.append([0] * x.ndim)
-  for idx in range(1, num_output):
-    st = [0] * x.ndim
-    st[axis] = sum(split[:idx])
-    starts.append(st)
-    en = list(x.shape)
-    en[axis] = sum(split[:idx])
-    ends.append(en)
-  ends.append(list(x.shape))
+    """ONNX version_13 Expand op."""
+    cls._prepare(node, inputs, onnx_expand)
+    return onnx_expand
+
 
-  return [lax.slice(x, start, end) for start, end in zip(starts, ends)]
+@functools.partial(jit, static_argnames="shape")
+def onnx_expand(*input_args, shape):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Expand for more details."""
+  data = input_args[0]
+  return data * jnp.ones(shape, dtype=data.dtype)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/sqrt.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/relu.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Sqrt operator."""
+"""Define ONNX Relu operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
+import jax
 from jax import jit
-from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Sqrt")
-class Sqrt(handler.Handler):
-  """Implementation of the ONNX Sqrt operator."""
+@handler.register_op("Relu")
+class Relu(handler.Handler):
+  """Implementation of the ONNX Relu operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,20 +53,29 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_13(
+  def version_6(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Sqrt op."""
-    cls._prepare(node, inputs, onnx_sqrt)
-    return onnx_sqrt
+    """ONNX version_6 Relu op."""
+    cls._prepare(node, inputs, onnx_relu)
+    return onnx_relu
+
+  @classmethod
+  def version_14(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_14 Relu op."""
+    cls._prepare(node, inputs, onnx_relu)
+    return onnx_relu
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_sqrt(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Sqrt."""
+def onnx_relu(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Relu for more details."""
   assert len(input_args) == 1
-  return jnp.sqrt(*input_args)
+  x = input_args[0]
+  return jax.nn.relu(x)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/squeeze.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/unsqueeze.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,45 +21,61 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Squeeze operator."""
+"""Define ONNX Unsqueeze operator."""
 from collections.abc import Callable, Sequence
 import functools
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Squeeze')
-class Squeeze(handler.Handler):
-  """Implementation of the ONNX Squeeze operator."""
+@handler.register_op('Unsqueeze')
+class Unsqueeze(handler.Handler):
+  """Implementation of the ONNX Unsqueeze operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    if len(inputs) == 1:
-      node.attrs_dict['axis'] = None
-    else:
+    if 'axes' in node.attrs:
+      node.attrs_dict['axis'] = node.attrs['axes']
+    if len(inputs) >= 2:
       node.attrs_dict['axis'] = tuple(inputs[1].tolist())
 
   @classmethod
+  def version_1(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_1 Unsqueeze op."""
+    cls._prepare(node, inputs, onnx_unsqueeze)
+    return onnx_unsqueeze
+
+  @classmethod
+  def version_11(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_11 Unsqueeze op."""
+    cls._prepare(node, inputs, onnx_unsqueeze)
+    return onnx_unsqueeze
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Squeeze op."""
-    cls._prepare(node, inputs, onnx_squeeze)
-    return onnx_squeeze
+    """ONNX version_13 Unsqueeze op."""
+    cls._prepare(node, inputs, onnx_unsqueeze)
+    return onnx_unsqueeze
 
 
 @functools.partial(jit, static_argnames='axis')
-def onnx_squeeze(*input_args, axis):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Squeeze."""
+def onnx_unsqueeze(*input_args, axis: list[int]):
+  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Unsqueeze."""
   x = input_args[0]
-  return jnp.squeeze(x, axis=axis)
+  return jnp.expand_dims(x, axis)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/sub.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sub.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,14 +51,30 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_7(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_7 Sub op."""
+    cls._prepare(node, inputs, onnx_sub)
+    return onnx_sub
+
+  @classmethod
+  def version_13(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_13 Sub op."""
+    cls._prepare(node, inputs, onnx_sub)
+    return onnx_sub
+
+  @classmethod
   def version_14(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_14 Sub op."""
     cls._prepare(node, inputs, onnx_sub)
     return onnx_sub
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/sum.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/sum.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,22 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
+  def version_8(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_8 Sum op."""
+    cls._prepare(node, inputs, onnx_sum)
+    return onnx_sum
+
+  @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
     """ONNX version_13 Sum op."""
     cls._prepare(node, inputs, onnx_sum)
     return onnx_sum
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/tanh.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/lessorequal.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Tanh operator."""
+"""Define ONNX LessOrEqual operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Tanh")
-class Tanh(handler.Handler):
-  """Implementation of the ONNX Tanh operator."""
+@handler.register_op("LessOrEqual")
+class LessOrEqual(handler.Handler):
+  """Implementation of the ONNX LessOrEqual operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,21 +53,28 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_13(
+  def version_12(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Tanh op."""
-    cls._prepare(node, inputs, onnx_tanh)
-    return onnx_tanh
+    """ONNX version_12 LessOrEqual op."""
+    cls._prepare(node, inputs, onnx_lessorequal)
+    return onnx_lessorequal
+
+  @classmethod
+  def version_16(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_16 LessOrEqual op."""
+    cls._prepare(node, inputs, onnx_lessorequal)
+    return onnx_lessorequal
 
 
 @functools.partial(jit, static_argnames=())
-def onnx_tanh(*input_args):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Tanh."""
-  assert len(input_args) == 1
-  x = input_args[0]
-  return jnp.tanh(x)
+def onnx_lessorequal(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#LessOrEqual for more details."""
+  assert len(input_args) == 2
+  return jnp.less_equal(input_args[0], input_args[1])
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/transpose.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/identity.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Transpose operator."""
+"""Define ONNX Identity operator."""
+# pylint: disable=unused-argument
+# pylint: disable=g-explicit-length-test
 from collections.abc import Callable, Sequence
 import functools
 import inspect
 from typing import Any
 
 from jax import jit
-from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op("Transpose")
-class Transpose(handler.Handler):
-  """Implementation of the ONNX Transpose operator."""
+@handler.register_op("Identity")
+class Identity(handler.Handler):
+  """Implementation of the ONNX Identity operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
     sig = inspect.signature(onnx_jax_impl)
     kwparams = [
@@ -51,21 +52,35 @@
         for param in sig.parameters.values()
         if param.kind == inspect.Parameter.KEYWORD_ONLY
     ]
     for name in kwparams:
       node.attrs_dict[name] = node.attrs.get(name, None)
 
   @classmethod
-  def version_13(
+  def version_1(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Transpose op."""
-    cls._prepare(node, inputs, onnx_transpose)
-    return onnx_transpose
+    """ONNX version_1 Identity op."""
+    cls._prepare(node, inputs, onnx_identity)
+    return onnx_identity
 
+  @classmethod
+  def version_16(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_16 Identity op."""
+    cls._prepare(node, inputs, onnx_identity)
+    return onnx_identity
 
-@functools.partial(jit, static_argnames="perm")
-def onnx_transpose(*input_args, perm):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Transpose."""
+  @classmethod
+  def version_19(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_19 Identity op."""
+    cls._prepare(node, inputs, onnx_identity)
+    return onnx_identity
+
+@functools.partial(jit, static_argnames=())
+def onnx_identity(*input_args):
+  """https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Identity for more details."""
   assert len(input_args) == 1
-  x = input_args[0]
-  return jnp.transpose(x, perm)
+  return [input_args[0]]
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/onnx_ops/unsqueeze.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/onnx_ops/div.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,45 +21,72 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define ONNX Unsqueeze operator."""
+"""Define ONNX Div operator."""
 from collections.abc import Callable, Sequence
 import functools
+import inspect
 from typing import Any
 
 from jax import jit
 from jax import numpy as jnp
 from jaxonnxruntime.core import handler
 from jaxonnxruntime.core import onnx_node
 
 
-@handler.register_op('Unsqueeze')
-class Unsqueeze(handler.Handler):
-  """Implementation of the ONNX Unsqueeze operator."""
+@handler.register_op("Div")
+class Div(handler.Handler):
+  """Implementation of the ONNX Div operator."""
 
   @classmethod
   def _prepare(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any], onnx_jax_impl: Any
   ):
-    if 'axes' in node.attrs:
-      node.attrs_dict['axis'] = node.attrs['axes']
-    if len(inputs) >= 2:
-      node.attrs_dict['axis'] = tuple(inputs[1].tolist())
+    sig = inspect.signature(onnx_jax_impl)
+    kwparams = [
+        param.name
+        for param in sig.parameters.values()
+        if param.kind == inspect.Parameter.KEYWORD_ONLY
+    ]
+    for name in kwparams:
+      node.attrs_dict[name] = node.attrs.get(name, None)
+
+  @classmethod
+  def version_7(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_7 Div op."""
+    cls._prepare(node, inputs, onnx_div)
+    return onnx_div
 
   @classmethod
   def version_13(
       cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
   ) -> Callable[..., Any]:
-    """ONNX version_13 Unsqueeze op."""
-    cls._prepare(node, inputs, onnx_unsqueeze)
-    return onnx_unsqueeze
+    """ONNX version_13 Div op."""
+    cls._prepare(node, inputs, onnx_div)
+    return onnx_div
 
+  @classmethod
+  def version_14(
+      cls, node: onnx_node.OnnxNode, inputs: Sequence[Any]
+  ) -> Callable[..., Any]:
+    """ONNX version_14 Div op."""
+    cls._prepare(node, inputs, onnx_div)
+    return onnx_div
 
-@functools.partial(jit, static_argnames='axis')
-def onnx_unsqueeze(*input_args, axis: list[int]):
-  """The impl for https://github.com/onnx/onnx/blob/v1.12.0/docs/Operators.md#Unsqueeze."""
-  x = input_args[0]
-  return jnp.expand_dims(x, axis)
+
+@functools.partial(jit, static_argnames=())
+def onnx_div(*input_args):
+  """The internal jax impl for onnx Div op."""
+  assert len(input_args) == 2
+  x, y = input_args
+  if jnp.issubdtype(x.dtype, jnp.integer) and jnp.issubdtype(
+      y.dtype, jnp.integer
+  ):
+    return jnp.floor_divide(x, y)
+  else:
+    return jnp.true_divide(x, y)
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/runner.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
 
   def _add_test(
       self,
       category: str,
       test_name: str,
       test_func: Callable[..., Any],
       report_item: list[Optional[Union[onnx.ModelProto, onnx.NodeProto]]],
-      devices: Iterable[str] = ('CPU', 'CUDA'),
+      devices: Iterable[str] = ('CPU', 'GPU', 'TPU'),
   ) -> None:
     """Add test to each device and category."""
     # We don't prepend the 'test_' prefix to improve greppability
     if not test_name.startswith('test_'):
       raise ValueError(f'Test name must start with test_: {test_name}')
 
     def add_device_test(device: str) -> None:
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime/version.py` & `jaxonnxruntime-0.1.0/jaxonnxruntime/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Current jaxonnxruntime version at head on Github."""
-__version__ = "0.0.2"
+__version__ = "0.1.0"
```

### Comparing `jaxonnxruntime-0.0.2/jaxonnxruntime.egg-info/SOURCES.txt` & `jaxonnxruntime-0.1.0/jaxonnxruntime.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -12,66 +12,86 @@
 docs/requirements.txt
 docs/_static/css/jaxonnxruntime_theme.css
 docs/examples/jaxonnxruntime-python-api.py
 examples/imagenet/imagenet_main.py
 jaxonnxruntime/__init__.py
 jaxonnxruntime/backend.py
 jaxonnxruntime/call_onnx.py
+jaxonnxruntime/config.py
 jaxonnxruntime/runner.py
 jaxonnxruntime/version.py
 jaxonnxruntime.egg-info/PKG-INFO
 jaxonnxruntime.egg-info/SOURCES.txt
 jaxonnxruntime.egg-info/dependency_links.txt
 jaxonnxruntime.egg-info/requires.txt
 jaxonnxruntime.egg-info/top_level.txt
 jaxonnxruntime/core/__init__.py
 jaxonnxruntime/core/handler.py
 jaxonnxruntime/core/onnx_graph.py
 jaxonnxruntime/core/onnx_node.py
+jaxonnxruntime/core/onnx_utils.py
 jaxonnxruntime/onnx_ops/__init__.py
 jaxonnxruntime/onnx_ops/abs.py
 jaxonnxruntime/onnx_ops/add.py
 jaxonnxruntime/onnx_ops/averagepool.py
 jaxonnxruntime/onnx_ops/batchnormalization.py
 jaxonnxruntime/onnx_ops/cast.py
+jaxonnxruntime/onnx_ops/ceil.py
 jaxonnxruntime/onnx_ops/concat.py
 jaxonnxruntime/onnx_ops/constant.py
 jaxonnxruntime/onnx_ops/constantofshape.py
 jaxonnxruntime/onnx_ops/conv.py
 jaxonnxruntime/onnx_ops/div.py
+jaxonnxruntime/onnx_ops/dropout.py
+jaxonnxruntime/onnx_ops/equal.py
 jaxonnxruntime/onnx_ops/exp.py
+jaxonnxruntime/onnx_ops/expand.py
 jaxonnxruntime/onnx_ops/flatten.py
 jaxonnxruntime/onnx_ops/gather.py
 jaxonnxruntime/onnx_ops/gemm.py
 jaxonnxruntime/onnx_ops/globalaveragepool.py
+jaxonnxruntime/onnx_ops/identity.py
+jaxonnxruntime/onnx_ops/if_op.py
 jaxonnxruntime/onnx_ops/leakyrelu.py
+jaxonnxruntime/onnx_ops/less.py
+jaxonnxruntime/onnx_ops/lessorequal.py
+jaxonnxruntime/onnx_ops/lrn.py
 jaxonnxruntime/onnx_ops/matmul.py
+jaxonnxruntime/onnx_ops/max.py
 jaxonnxruntime/onnx_ops/maxpool.py
 jaxonnxruntime/onnx_ops/mul.py
+jaxonnxruntime/onnx_ops/neg.py
 jaxonnxruntime/onnx_ops/nonzero.py
+jaxonnxruntime/onnx_ops/onehot.py
+jaxonnxruntime/onnx_ops/or_op.py
 jaxonnxruntime/onnx_ops/pad.py
 jaxonnxruntime/onnx_ops/pow.py
+jaxonnxruntime/onnx_ops/range.py
+jaxonnxruntime/onnx_ops/reciprocal.py
 jaxonnxruntime/onnx_ops/reducemax.py
 jaxonnxruntime/onnx_ops/reducemean.py
 jaxonnxruntime/onnx_ops/reducesum.py
 jaxonnxruntime/onnx_ops/relu.py
 jaxonnxruntime/onnx_ops/reshape.py
 jaxonnxruntime/onnx_ops/shape.py
+jaxonnxruntime/onnx_ops/sigmoid.py
 jaxonnxruntime/onnx_ops/slice.py
 jaxonnxruntime/onnx_ops/softmax.py
 jaxonnxruntime/onnx_ops/split.py
 jaxonnxruntime/onnx_ops/sqrt.py
 jaxonnxruntime/onnx_ops/squeeze.py
 jaxonnxruntime/onnx_ops/sub.py
 jaxonnxruntime/onnx_ops/sum.py
 jaxonnxruntime/onnx_ops/tanh.py
 jaxonnxruntime/onnx_ops/transpose.py
 jaxonnxruntime/onnx_ops/unsqueeze.py
+jaxonnxruntime/onnx_ops/where.py
 tests/call_onnx_test.py
-tests/onnx_models_test.py
 tests/onnx_ops_test.py
 tests/run_all_tests.sh
 tests/core/handler_test.py
 tests/core/onnx_graph_test.py
 tests/core/onnx_node_test.py
+tests/onnx_ops/dropout_test.py
+tests/onnx_ops/onehot_test.py
 tools/analyze_model.py
 tools/op_code_generator.py
```

### Comparing `jaxonnxruntime-0.0.2/pylintrc` & `jaxonnxruntime-0.1.0/pylintrc`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/pyproject.toml` & `jaxonnxruntime-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 authors = [
     {name = "Jaxonnxruntime team", email = "jaxonnxruntime-dev@google.com"},
 ]
 dependencies = [
     "numpy",
     "jax",
     "jaxlib",
-    "orbax_export",
-    "onnx==1.12.0",  # Please keep this as the last line since onnx request old protobuf lib.
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.7",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 all = [
+    "onnx==1.12.0",  # Please keep this as the last line since onnx request old protobuf lib.
 ]
 
 testing = [
     "mypy",
     "pytest",
     "pytest-cov",
     "pytest-custom_exit_code",
```

### Comparing `jaxonnxruntime-0.0.2/tests/call_onnx_test.py` & `jaxonnxruntime-0.1.0/tests/call_onnx_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     graph_def = GraphProto(
         node=[node_abs],
         name='abs_graph',
         input=[input_tensor],
         output=[output_tensor],
     )
     model_proto = ModelProto(graph=graph_def, producer_name='onnx-example')
-    jax_func, model_params = call_onnx.call_onnx(model_proto, [x])
+    jax_func, model_params = call_onnx.call_onnx_model(model_proto, [x])
     results = jax_func(model_params, [x])
     expect = [np.array([2.0, 1.0, 3.0], dtype=np.float32)]
     np.testing.assert_array_equal(results, expect)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `jaxonnxruntime-0.0.2/tests/core/handler_test.py` & `jaxonnxruntime-0.1.0/tests/core/handler_test.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/tests/core/onnx_graph_test.py` & `jaxonnxruntime-0.1.0/tests/core/onnx_graph_test.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/tests/core/onnx_node_test.py` & `jaxonnxruntime-0.1.0/tests/core/onnx_node_test.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/tests/run_all_tests.sh` & `jaxonnxruntime-0.1.0/tests/run_all_tests.sh`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/tools/analyze_model.py` & `jaxonnxruntime-0.1.0/tools/analyze_model.py`

 * *Files identical despite different names*

### Comparing `jaxonnxruntime-0.0.2/tools/op_code_generator.py` & `jaxonnxruntime-0.1.0/tools/op_code_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 def update_onnx_ops_init_file(op_name):
   """Update onnx_ops/__init_.py with the created op."""
   init_py_file = os.path.join(root_dir, '__init__.py')
   with open(init_py_file, 'r') as f:
     existing_imports = f.read()
 
-  new_import = f'from . import {op_name.lower()}'
+  new_import = f'from . import {op_name.lower()} as {op_name.lower()}'
   if new_import in existing_imports:
     logging.info('Already have %s in onnx_ops/__init__.py.', op_name)
     return
 
   # Split the existing imports.
   initial_imports = existing_imports.split('from . import ')[0]
   onnx_op_imports = existing_imports[len(initial_imports) :]
```

