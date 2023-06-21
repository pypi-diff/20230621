# Comparing `tmp/tart_lib-0.1.0.tar.gz` & `tmp/tart_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tart_lib-0.1.0.tar", max compression
+gzip compressed data, was "tart_lib-0.1.1.tar", max compression
```

## Comparing `tart_lib-0.1.0.tar` & `tart_lib-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      549 2023-05-03 00:36:39.771084 tart_lib-0.1.0/README.md
--rw-r--r--   0        0        0      676 2023-05-27 17:34:08.984561 tart_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 16:34:41.260056 tart_lib-0.1.0/tart/__init__.py
--rw-r--r--   0        0        0      151 2023-04-28 16:34:41.260166 tart_lib-0.1.0/tart/data/.gitignore
--rw-r--r--   0        0        0      189 2023-04-28 16:34:41.260342 tart_lib-0.1.0/tart/data/example/embed/raw/example_0.json
--rw-r--r--   0        0        0      189 2023-04-28 16:34:41.260401 tart_lib-0.1.0/tart/data/example/embed/raw/example_1.json
--rw-r--r--   0        0        0      212 2023-04-28 16:34:41.260470 tart_lib-0.1.0/tart/data/example/embed/raw/example_2.json
--rw-r--r--   0        0        0      278 2023-04-28 16:34:41.260566 tart_lib-0.1.0/tart/data/example/embed/raw/example_3.json
--rw-r--r--   0        0        0      189 2023-04-28 16:34:41.260776 tart_lib-0.1.0/tart/data/example/test/raw/g1.json
--rw-r--r--   0        0        0      189 2023-04-28 16:34:41.260841 tart_lib-0.1.0/tart/data/example/test/raw/g2.json
--rw-r--r--   0        0        0      212 2023-04-28 16:34:41.260973 tart_lib-0.1.0/tart/data/example/train/raw/g1.json
--rw-r--r--   0        0        0      278 2023-04-28 16:34:41.261032 tart_lib-0.1.0/tart/data/example/train/raw/g2.json
--rw-r--r--   0        0        0        0 2023-04-28 16:34:41.261093 tart_lib-0.1.0/tart/example/__init__.py
--rw-r--r--   0        0        0      444 2023-05-21 06:24:54.106099 tart_lib-0.1.0/tart/example/learn.py
--rw-r--r--   0        0        0      635 2023-05-02 22:09:47.690893 tart_lib-0.1.0/tart/example/predict.py
--rw-r--r--   0        0        0      449 2023-05-17 05:21:50.409874 tart_lib-0.1.0/tart/example/tart-config.json
--rw-r--r--   0        0        0        0 2023-04-28 16:34:41.261386 tart_lib-0.1.0/tart/inference/__init__.py
--rw-r--r--   0        0        0     9202 2023-05-27 16:14:20.431795 tart_lib-0.1.0/tart/inference/embed.py
--rw-r--r--   0        0        0     7560 2023-05-27 16:29:22.084402 tart_lib-0.1.0/tart/inference/predict.py
--rw-r--r--   0        0        0        0 2023-04-28 16:34:41.261698 tart_lib-0.1.0/tart/representation/__init__.py
--rw-r--r--   0        0        0     7972 2023-05-27 15:49:10.773030 tart_lib-0.1.0/tart/representation/config.py
--rw-r--r--   0        0        0    10911 2023-05-27 15:27:36.124050 tart_lib-0.1.0/tart/representation/dataset.py
--rw-r--r--   0        0        0     2883 2023-05-27 15:49:25.321433 tart_lib-0.1.0/tart/representation/encoders.py
--rw-r--r--   0        0        0    11220 2023-05-27 15:49:25.394930 tart_lib-0.1.0/tart/representation/models.py
--rw-r--r--   0        0        0     9025 2023-05-27 15:40:23.548106 tart_lib-0.1.0/tart/representation/test.py
--rw-r--r--   0        0        0     7744 2023-05-27 16:06:49.913898 tart_lib-0.1.0/tart/representation/train.py
--rw-r--r--   0        0        0        0 2023-04-28 16:34:41.262341 tart_lib-0.1.0/tart/utils/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-04 23:28:36.655307 tart_lib-0.1.0/tart/utils/config_utils.py
--rw-r--r--   0        0        0     3391 2023-05-27 16:09:38.404192 tart_lib-0.1.0/tart/utils/graph_utils.py
--rw-r--r--   0        0        0       94 2023-05-02 22:15:09.179104 tart_lib-0.1.0/tart/utils/infer_utils.py
--rw-r--r--   0        0        0     2659 2023-05-05 00:26:18.104754 tart_lib-0.1.0/tart/utils/model_utils.py
--rw-r--r--   0        0        0     1363 2023-05-04 23:30:40.166599 tart_lib-0.1.0/tart/utils/tart_utils.py
--rw-r--r--   0        0        0     2914 2023-05-17 04:51:08.157530 tart_lib-0.1.0/tart/utils/train_utils.py
--rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 tart_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-21 06:40:35.491753 tart_lib-0.1.1/LICENSE
+-rw-r--r--   0        0        0      549 2023-06-21 06:40:35.491753 tart_lib-0.1.1/README.md
+-rw-r--r--   0        0        0      741 2023-06-21 06:40:35.503753 tart_lib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 06:40:35.503753 tart_lib-0.1.1/tart/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/cli/__init__.py
+-rw-r--r--   0        0        0     4703 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/cli/cli.py
+-rw-r--r--   0        0        0      151 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/.gitignore
+-rw-r--r--   0        0        0      189 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/example/embed/raw/example_0.json
+-rw-r--r--   0        0        0      189 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/example/embed/raw/example_1.json
+-rw-r--r--   0        0        0      212 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/example/embed/raw/example_2.json
+-rw-r--r--   0        0        0      278 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/example/embed/raw/example_3.json
+-rw-r--r--   0        0        0      189 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/example/test/raw/g1.json
+-rw-r--r--   0        0        0      189 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/example/test/raw/g2.json
+-rw-r--r--   0        0        0      212 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/example/train/raw/g1.json
+-rw-r--r--   0        0        0      278 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/data/example/train/raw/g2.json
+-rw-r--r--   0        0        0        0 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/example/__init__.py
+-rw-r--r--   0        0        0      444 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/example/learn.py
+-rw-r--r--   0        0        0      635 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/example/predict.py
+-rw-r--r--   0        0        0      449 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/example/tart-config.json
+-rw-r--r--   0        0        0        0 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/inference/__init__.py
+-rw-r--r--   0        0        0     9202 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/inference/embed.py
+-rw-r--r--   0        0        0     7560 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/inference/predict.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/representation/__init__.py
+-rw-r--r--   0        0        0     7972 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/representation/config.py
+-rw-r--r--   0        0        0    10911 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/representation/dataset.py
+-rw-r--r--   0        0        0     2883 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/representation/encoders.py
+-rw-r--r--   0        0        0    11220 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/representation/models.py
+-rw-r--r--   0        0        0     9025 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/representation/test.py
+-rw-r--r--   0        0        0     7744 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/representation/train.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/utils/__init__.py
+-rw-r--r--   0        0        0     1069 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/utils/config_utils.py
+-rw-r--r--   0        0        0     3391 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/utils/graph_utils.py
+-rw-r--r--   0        0        0       94 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/utils/infer_utils.py
+-rw-r--r--   0        0        0     2659 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/utils/model_utils.py
+-rw-r--r--   0        0        0     1363 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/utils/tart_utils.py
+-rw-r--r--   0        0        0     2914 2023-06-21 06:40:35.507753 tart_lib-0.1.1/tart/utils/train_utils.py
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 tart_lib-0.1.1/PKG-INFO
```

### Comparing `tart_lib-0.1.0/README.md` & `tart_lib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/pyproject.toml` & `tart_lib-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tart-lib"
 packages = [{ include = "tart" }]
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["manishshettym <manishs@berkeley.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.0.1"
@@ -16,17 +16,21 @@
 networkx = "^3.1"
 matplotlib = "^3.7.1"
 openpyxl = "^3.1.2"
 pycodestyle = "^2.10.0"
 rich = "^13.3.5"
 tensorboard = "^2.12.2"
 test-tube = "^0.7.5"
+typer = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.0.0"
 pytest-cov = ">=2.10.0"
 pytest-xdist = ">=2.0.0"
 black = "^23.1.0"
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+tart = "tart.cli.cli:app"
```

### Comparing `tart_lib-0.1.0/tart/example/predict.py` & `tart_lib-0.1.1/tart/example/predict.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/inference/embed.py` & `tart_lib-0.1.1/tart/inference/embed.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/inference/predict.py` & `tart_lib-0.1.1/tart/inference/predict.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/representation/config.py` & `tart_lib-0.1.1/tart/representation/config.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/representation/dataset.py` & `tart_lib-0.1.1/tart/representation/dataset.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/representation/encoders.py` & `tart_lib-0.1.1/tart/representation/encoders.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/representation/models.py` & `tart_lib-0.1.1/tart/representation/models.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/representation/test.py` & `tart_lib-0.1.1/tart/representation/test.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/representation/train.py` & `tart_lib-0.1.1/tart/representation/train.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/utils/config_utils.py` & `tart_lib-0.1.1/tart/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/utils/graph_utils.py` & `tart_lib-0.1.1/tart/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/utils/model_utils.py` & `tart_lib-0.1.1/tart/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/utils/tart_utils.py` & `tart_lib-0.1.1/tart/utils/tart_utils.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/tart/utils/train_utils.py` & `tart_lib-0.1.1/tart/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `tart_lib-0.1.0/PKG-INFO` & `tart_lib-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tart-lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: manishshettym
 Author-email: manishs@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,14 +17,15 @@
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pycodestyle (>=2.10.0,<3.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: tensorboard (>=2.12.2,<3.0.0)
 Requires-Dist: test-tube (>=0.7.5,<0.8.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # <img src="docs/_static/tart.svg" alt="tart logo" height="52" align="absbottom" align="left"> [`tart`](): tensor abstracted relations and topologies
 
 [![pytest](https://github.com/tart-proj/tart/actions/workflows/pytest.yml/badge.svg)](https://github.com/tart-proj/tart/actions/workflows/pytest.yml)
 [![Documentation Status](https://readthedocs.org/projects/tart/badge/?version=latest)](https://tart.readthedocs.io/en/latest/?badge=latest)
```

