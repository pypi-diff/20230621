# Comparing `tmp/ml-rwkv-0.0.1.tar.gz` & `tmp/ml-rwkv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-rwkv-0.0.1.tar", last modified: Wed Jun 21 03:32:12 2023, max compression
+gzip compressed data, was "ml-rwkv-0.0.2.tar", last modified: Wed Jun 21 19:27:35 2023, max compression
```

## Comparing `ml-rwkv-0.0.1.tar` & `ml-rwkv-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-21 03:32:12.194709 ml-rwkv-0.0.1/
--rw-r--r--   0 ben        (501) staff       (20)     1071 2023-06-16 04:42:26.000000 ml-rwkv-0.0.1/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)      104 2023-06-16 04:48:57.000000 ml-rwkv-0.0.1/MANIFEST.in
--rw-r--r--   0 ben        (501) staff       (20)     1722 2023-06-21 03:32:12.194760 ml-rwkv-0.0.1/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1174 2023-06-21 03:23:05.000000 ml-rwkv-0.0.1/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-21 03:32:12.192217 ml-rwkv-0.0.1/ml_rwkv.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     1722 2023-06-21 03:32:12.000000 ml-rwkv-0.0.1/ml_rwkv.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      555 2023-06-21 03:32:12.000000 ml-rwkv-0.0.1/ml_rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-06-21 03:32:12.000000 ml-rwkv-0.0.1/ml_rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       39 2023-06-21 03:32:12.000000 ml-rwkv-0.0.1/ml_rwkv.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)       45 2023-06-21 03:32:12.000000 ml-rwkv-0.0.1/ml_rwkv.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)        5 2023-06-21 03:32:12.000000 ml-rwkv-0.0.1/ml_rwkv.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)     1611 2023-06-21 03:23:05.000000 ml-rwkv-0.0.1/pyproject.toml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-21 03:32:12.192747 ml-rwkv-0.0.1/rwkv/
--rw-r--r--   0 ben        (501) staff       (20)       22 2023-06-16 04:44:40.000000 ml-rwkv-0.0.1/rwkv/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)    13220 2023-06-21 03:22:58.000000 ml-rwkv-0.0.1/rwkv/model.py
--rw-r--r--   0 ben        (501) staff       (20)     2210 2023-06-21 03:22:58.000000 ml-rwkv-0.0.1/rwkv/run.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-21 03:32:12.193017 ml-rwkv-0.0.1/rwkv/triton/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-06-16 05:15:59.000000 ml-rwkv-0.0.1/rwkv/triton/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)      502 2023-06-21 03:23:05.000000 ml-rwkv-0.0.1/rwkv/triton/utils.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-21 03:32:12.193292 ml-rwkv-0.0.1/rwkv/triton/wkv/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-06-21 03:23:05.000000 ml-rwkv-0.0.1/rwkv/triton/wkv/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)    11492 2023-06-21 03:23:05.000000 ml-rwkv-0.0.1/rwkv/triton/wkv/vanilla.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-21 03:32:12.193808 ml-rwkv-0.0.1/rwkv/wkv/
--rw-r--r--   0 ben        (501) staff       (20)     2246 2023-06-21 03:23:05.000000 ml-rwkv-0.0.1/rwkv/wkv/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     6271 2023-06-21 03:22:58.000000 ml-rwkv-0.0.1/rwkv/wkv/eps.py
--rw-r--r--   0 ben        (501) staff       (20)     7658 2023-06-21 03:23:05.000000 ml-rwkv-0.0.1/rwkv/wkv/log.py
--rw-r--r--   0 ben        (501) staff       (20)     5101 2023-06-21 03:23:05.000000 ml-rwkv-0.0.1/rwkv/wkv/vanilla.py
--rw-r--r--   0 ben        (501) staff       (20)      183 2023-06-21 03:32:12.194958 ml-rwkv-0.0.1/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)     1229 2023-06-21 03:32:03.000000 ml-rwkv-0.0.1/setup.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-21 03:32:12.194596 ml-rwkv-0.0.1/tests/
--rw-r--r--   0 ben        (501) staff       (20)     3109 2023-06-17 22:28:24.000000 ml-rwkv-0.0.1/tests/test_eps_wkv.py
--rw-r--r--   0 ben        (501) staff       (20)     3438 2023-06-19 13:11:51.000000 ml-rwkv-0.0.1/tests/test_log_wkv.py
--rw-r--r--   0 ben        (501) staff       (20)     3329 2023-06-19 13:11:51.000000 ml-rwkv-0.0.1/tests/test_vanilla_wkv.py
--rw-r--r--   0 ben        (501) staff       (20)     2297 2023-06-21 03:23:42.000000 ml-rwkv-0.0.1/tests/test_wkv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.292059 ml-rwkv-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-21 19:27:35.292059 ml-rwkv-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/ml_rwkv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/rwkv/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/rwkv/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/triton/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/rwkv/triton/wkv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/triton/wkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/triton/wkv/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/rwkv/wkv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/wkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/wkv/eps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/wkv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/wkv/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 19:27:35.292059 ml-rwkv-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.292059 ml-rwkv-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/tests/test_eps_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/tests/test_log_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/tests/test_vanilla_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/tests/test_wkv.py
```

### Comparing `ml-rwkv-0.0.1/LICENSE` & `ml-rwkv-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/PKG-INFO` & `ml-rwkv-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 Metadata-Version: 2.1
 Name: ml-rwkv
-Version: 0.0.1
+Version: 0.0.2
 Summary: RWKV implementation that is friendly with `ml-starter`
 Home-page: https://github.com/codekansas/rwkv
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 # RWKV
 
 This repository contains my implementation of the pretrained RWKV model, with numerically-stable Triton kernels and code for doing LoRA fine-tuning.
 
-For an explanation of the math, see [this accompanying blog post](https://ben.bolte.cc/rwkv).
+For an explanation of the math, see [this accompanying blog post](https://ben.bolte.cc/rwkv-model).
+
+## Getting Started
+
+Install the package:
+
+```
+pip install ml-rwkv
+```
+
+Generate code:
+
+```
+rwkv 169m "Scientists recently discovered a herd of Chinese-speaking goats. To their surprise,"
+```
 
 ## WKV Computations
 
 This repo currently contains 3 different implementations of the WKV computation:
 
 1. Vanilla
 2. Eps
```

### Comparing `ml-rwkv-0.0.1/ml_rwkv.egg-info/PKG-INFO` & `ml-rwkv-0.0.2/ml_rwkv.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 Metadata-Version: 2.1
 Name: ml-rwkv
-Version: 0.0.1
+Version: 0.0.2
 Summary: RWKV implementation that is friendly with `ml-starter`
 Home-page: https://github.com/codekansas/rwkv
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 # RWKV
 
 This repository contains my implementation of the pretrained RWKV model, with numerically-stable Triton kernels and code for doing LoRA fine-tuning.
 
-For an explanation of the math, see [this accompanying blog post](https://ben.bolte.cc/rwkv).
+For an explanation of the math, see [this accompanying blog post](https://ben.bolte.cc/rwkv-model).
+
+## Getting Started
+
+Install the package:
+
+```
+pip install ml-rwkv
+```
+
+Generate code:
+
+```
+rwkv 169m "Scientists recently discovered a herd of Chinese-speaking goats. To their surprise,"
+```
 
 ## WKV Computations
 
 This repo currently contains 3 different implementations of the WKV computation:
 
 1. Vanilla
 2. Eps
```

### Comparing `ml-rwkv-0.0.1/ml_rwkv.egg-info/SOURCES.txt` & `ml-rwkv-0.0.2/ml_rwkv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/pyproject.toml` & `ml-rwkv-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/rwkv/model.py` & `ml-rwkv-0.0.2/rwkv/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     pip install tokenizers
 
 Additionally, using the training mode CUDA kernel requires installing ``triton``:
 
 .. code-block:: bash
 
-    pip install
+    pip install triton
 
 The choices for the model key are:
 
 - ``"169m"``
 - ``"430m"``
 - ``"1.5b"``
 - ``"3b"``
```

### Comparing `ml-rwkv-0.0.1/rwkv/run.py` & `ml-rwkv-0.0.2/rwkv/run.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/rwkv/triton/wkv/vanilla.py` & `ml-rwkv-0.0.2/rwkv/triton/wkv/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/rwkv/wkv/__init__.py` & `ml-rwkv-0.0.2/rwkv/wkv/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/rwkv/wkv/eps.py` & `ml-rwkv-0.0.2/rwkv/wkv/eps.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/rwkv/wkv/log.py` & `ml-rwkv-0.0.2/rwkv/wkv/log.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/rwkv/wkv/vanilla.py` & `ml-rwkv-0.0.2/rwkv/wkv/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/setup.py` & `ml-rwkv-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,10 +29,10 @@
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     python_requires=">=3.10",
     install_requires=["ml-starter", "tokenizers"],
     tests_require=["ml-starter[dev]"],
-    extras_require={"dev": ["ml-starter[dev]"]},
+    extras_require={"dev": ["ml-starter[dev]"], "docs": ["ml-starter[docs]"]},
     package_data={"rwkv": ["py.typed"]},
 )
```

### Comparing `ml-rwkv-0.0.1/tests/test_eps_wkv.py` & `ml-rwkv-0.0.2/tests/test_eps_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/tests/test_log_wkv.py` & `ml-rwkv-0.0.2/tests/test_log_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/tests/test_vanilla_wkv.py` & `ml-rwkv-0.0.2/tests/test_vanilla_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.1/tests/test_wkv.py` & `ml-rwkv-0.0.2/tests/test_wkv.py`

 * *Files identical despite different names*

