# Comparing `tmp/acids-rave-2.2.0.tar.gz` & `tmp/acids-rave-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-rave-2.2.0.tar", last modified: Fri Jun 16 14:41:07 2023, max compression
+gzip compressed data, was "acids-rave-2.2.1.tar", last modified: Wed Jun 21 08:57:09 2023, max compression
```

## Comparing `acids-rave-2.2.0.tar` & `acids-rave-2.2.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:41:07.388063 acids-rave-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-06-16 14:38:15.000000 acids-rave-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 14:38:15.000000 acids-rave-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-16 14:41:07.388063 acids-rave-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-16 14:38:15.000000 acids-rave-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:41:07.380063 acids-rave-2.2.0/acids_rave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-16 14:41:07.000000 acids-rave-2.2.0/acids_rave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-16 14:41:07.000000 acids-rave-2.2.0/acids_rave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:41:07.000000 acids-rave-2.2.0/acids_rave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 14:41:07.000000 acids-rave-2.2.0/acids_rave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 14:41:07.000000 acids-rave-2.2.0/acids_rave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 14:41:07.000000 acids-rave-2.2.0/acids_rave.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:41:07.380063 acids-rave-2.2.0/rave/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:41:07.384063 acids-rave-2.2.0/rave/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/adain.gin
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/causal.gin
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/descript_discriminator.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/discrete.gin
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/hybrid.gin
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/noise.gin
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/onnx.gin
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/raspberry.gin
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/snake.gin
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/spectral_discriminator.gin
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/spherical.gin
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/v1.gin
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/v2.gin
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/v3.gin
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/configs/wasserstein.gin
--rw-r--r--   0 runner    (1001) docker     (123)    14713 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/descript_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/pqmf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/quantization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-16 14:38:15.000000 acids-rave-2.2.0/rave/resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-16 14:38:15.000000 acids-rave-2.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:41:07.384063 acids-rave-2.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:38:15.000000 acids-rave-2.2.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-16 14:38:15.000000 acids-rave-2.2.0/scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-16 14:38:15.000000 acids-rave-2.2.0/scripts/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-16 14:38:15.000000 acids-rave-2.2.0/scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-16 14:38:15.000000 acids-rave-2.2.0/scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-16 14:38:15.000000 acids-rave-2.2.0/scripts/remote_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-16 14:38:15.000000 acids-rave-2.2.0/scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:41:07.388063 acids-rave-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-16 14:38:15.000000 acids-rave-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:41:07.384063 acids-rave-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:38:15.000000 acids-rave-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-16 14:38:15.000000 acids-rave-2.2.0/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-16 14:38:15.000000 acids-rave-2.2.0/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-16 14:38:15.000000 acids-rave-2.2.0/tests/test_residual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.240671 acids-rave-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-06-21 08:53:56.000000 acids-rave-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 08:53:56.000000 acids-rave-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 08:57:09.240671 acids-rave-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-21 08:53:56.000000 acids-rave-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.232671 acids-rave-2.2.1/acids_rave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.232671 acids-rave-2.2.1/rave/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.236671 acids-rave-2.2.1/rave/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/adain.gin
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/causal.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/descript_discriminator.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/discrete.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/discrete_v3.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/hybrid.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/noise.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/onnx.gin
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/raspberry.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/snake.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/spectral_discriminator.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/spherical.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/v1.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/v2.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/v3.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/wasserstein.gin
+-rw-r--r--   0 runner    (1001) docker     (123)    14713 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/descript_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/pqmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 08:53:56.000000 acids-rave-2.2.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.236671 acids-rave-2.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/remote_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:57:09.240671 acids-rave-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 08:53:56.000000 acids-rave-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.240671 acids-rave-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:56.000000 acids-rave-2.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-21 08:53:56.000000 acids-rave-2.2.1/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-21 08:53:56.000000 acids-rave-2.2.1/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-21 08:53:56.000000 acids-rave-2.2.1/tests/test_residual.py
```

### Comparing `acids-rave-2.2.0/LICENSE` & `acids-rave-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/PKG-INFO` & `acids-rave-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-rave
-Version: 2.2.0
+Version: 2.2.1
 Summary: RAVE: a Realtime Audio Variatione autoEncoder
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-rave Version: 2.2.0 Summary: RAVE: a Realtime
+Metadata-Version: 2.1 Name: acids-rave Version: 2.2.1 Summary: RAVE: a Realtime
 Audio Variatione autoEncoder Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE ![rave_logo](docs/rave.png) # RAVE: Realtime Audio
 Variational autoEncoder Official implementation of _RAVE: A variational
 autoencoder for fast and high-quality neural audio synthesis_ ([article link]
```

### Comparing `acids-rave-2.2.0/README.md` & `acids-rave-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/acids_rave.egg-info/PKG-INFO` & `acids-rave-2.2.1/acids_rave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-rave
-Version: 2.2.0
+Version: 2.2.1
 Summary: RAVE: a Realtime Audio Variatione autoEncoder
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-rave Version: 2.2.0 Summary: RAVE: a Realtime
+Metadata-Version: 2.1 Name: acids-rave Version: 2.2.1 Summary: RAVE: a Realtime
 Audio Variatione autoEncoder Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE ![rave_logo](docs/rave.png) # RAVE: Realtime Audio
 Variational autoEncoder Official implementation of _RAVE: A variational
 autoencoder for fast and high-quality neural audio synthesis_ ([article link]
```

### Comparing `acids-rave-2.2.0/acids_rave.egg-info/SOURCES.txt` & `acids-rave-2.2.1/acids_rave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 rave/pqmf.py
 rave/quantization.py
 rave/resampler.py
 rave/configs/adain.gin
 rave/configs/causal.gin
 rave/configs/descript_discriminator.gin
 rave/configs/discrete.gin
+rave/configs/discrete_v3.gin
 rave/configs/hybrid.gin
 rave/configs/noise.gin
 rave/configs/onnx.gin
 rave/configs/raspberry.gin
 rave/configs/snake.gin
 rave/configs/spectral_discriminator.gin
 rave/configs/spherical.gin
```

### Comparing `acids-rave-2.2.0/rave/blocks.py` & `acids-rave-2.2.1/rave/blocks.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/configs/discrete.gin` & `acids-rave-2.2.1/rave/configs/discrete.gin`

 * *Files 8% similar despite different names*

```diff
@@ -43,7 +43,12 @@
     phase_1_duration = %PHASE_1_DURATION
     warmup_quantize = -1
     discriminator = @discriminator.CombineDiscriminators
     gan_loss = @core.hinge_gan
     valid_signal_crop = True
     num_skipped_features = 0
     update_discriminator_every = 4
+
+rave.BetaWarmupCallback:
+    initial_value = .1
+    target_value = .1
+    warmup_len = 1
```

### Comparing `acids-rave-2.2.0/rave/configs/hybrid.gin` & `acids-rave-2.2.1/rave/configs/hybrid.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/configs/v1.gin` & `acids-rave-2.2.1/rave/configs/v1.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/configs/v2.gin` & `acids-rave-2.2.1/rave/configs/v2.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/configs/wasserstein.gin` & `acids-rave-2.2.1/rave/configs/wasserstein.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/core.py` & `acids-rave-2.2.1/rave/core.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/dataset.py` & `acids-rave-2.2.1/rave/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/descript_discriminator.py` & `acids-rave-2.2.1/rave/descript_discriminator.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/discriminator.py` & `acids-rave-2.2.1/rave/discriminator.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/model.py` & `acids-rave-2.2.1/rave/model.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/pqmf.py` & `acids-rave-2.2.1/rave/pqmf.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/quantization.py` & `acids-rave-2.2.1/rave/quantization.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/rave/resampler.py` & `acids-rave-2.2.1/rave/resampler.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/scripts/export.py` & `acids-rave-2.2.1/scripts/export.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/scripts/export_onnx.py` & `acids-rave-2.2.1/scripts/export_onnx.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/scripts/main_cli.py` & `acids-rave-2.2.1/scripts/main_cli.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/scripts/preprocess.py` & `acids-rave-2.2.1/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/scripts/remote_dataset.py` & `acids-rave-2.2.1/scripts/remote_dataset.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/scripts/train.py` & `acids-rave-2.2.1/scripts/train.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/setup.py` & `acids-rave-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/tests/test_configs.py` & `acids-rave-2.2.1/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/tests/test_resampler.py` & `acids-rave-2.2.1/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.0/tests/test_residual.py` & `acids-rave-2.2.1/tests/test_residual.py`

 * *Files identical despite different names*

