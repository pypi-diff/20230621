# Comparing `tmp/acids-rave-2.2.1.tar.gz` & `tmp/acids-rave-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-rave-2.2.1.tar", last modified: Wed Jun 21 08:57:09 2023, max compression
+gzip compressed data, was "acids-rave-2.2.2.tar", last modified: Wed Jun 21 13:35:21 2023, max compression
```

## Comparing `acids-rave-2.2.1.tar` & `acids-rave-2.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.240671 acids-rave-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-06-21 08:53:56.000000 acids-rave-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 08:53:56.000000 acids-rave-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 08:57:09.240671 acids-rave-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-21 08:53:56.000000 acids-rave-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.232671 acids-rave-2.2.1/acids_rave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 08:57:09.000000 acids-rave-2.2.1/acids_rave.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.232671 acids-rave-2.2.1/rave/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.236671 acids-rave-2.2.1/rave/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/adain.gin
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/causal.gin
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/descript_discriminator.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/discrete.gin
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/discrete_v3.gin
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/hybrid.gin
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/noise.gin
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/onnx.gin
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/raspberry.gin
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/snake.gin
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/spectral_discriminator.gin
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/spherical.gin
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/v1.gin
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/v2.gin
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/v3.gin
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/configs/wasserstein.gin
--rw-r--r--   0 runner    (1001) docker     (123)    14713 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/descript_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/pqmf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/quantization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 08:53:56.000000 acids-rave-2.2.1/rave/resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 08:53:56.000000 acids-rave-2.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.236671 acids-rave-2.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/remote_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-21 08:53:56.000000 acids-rave-2.2.1/scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:57:09.240671 acids-rave-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 08:53:56.000000 acids-rave-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:09.240671 acids-rave-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:53:56.000000 acids-rave-2.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-21 08:53:56.000000 acids-rave-2.2.1/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-21 08:53:56.000000 acids-rave-2.2.1/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-21 08:53:56.000000 acids-rave-2.2.1/tests/test_residual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:21.964094 acids-rave-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-06-21 13:30:33.000000 acids-rave-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 13:30:33.000000 acids-rave-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 13:35:21.964094 acids-rave-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-21 13:30:33.000000 acids-rave-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:21.956094 acids-rave-2.2.2/acids_rave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 13:35:21.000000 acids-rave-2.2.2/acids_rave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 13:35:21.000000 acids-rave-2.2.2/acids_rave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:35:21.000000 acids-rave-2.2.2/acids_rave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 13:35:21.000000 acids-rave-2.2.2/acids_rave.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 13:35:21.000000 acids-rave-2.2.2/acids_rave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 13:35:21.000000 acids-rave-2.2.2/acids_rave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:21.960094 acids-rave-2.2.2/rave/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:21.960094 acids-rave-2.2.2/rave/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/adain.gin
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/causal.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/descript_discriminator.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/discrete.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/discrete_v3.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/hybrid.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/noise.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/onnx.gin
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/raspberry.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/snake.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/spectral_discriminator.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/spherical.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/v1.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/v2.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/v3.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/configs/wasserstein.gin
+-rw-r--r--   0 runner    (1001) docker     (123)    14713 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/descript_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/pqmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 13:30:33.000000 acids-rave-2.2.2/rave/resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 13:30:33.000000 acids-rave-2.2.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:21.964094 acids-rave-2.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:30:33.000000 acids-rave-2.2.2/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-06-21 13:30:33.000000 acids-rave-2.2.2/scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-21 13:30:33.000000 acids-rave-2.2.2/scripts/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-21 13:30:33.000000 acids-rave-2.2.2/scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-21 13:30:33.000000 acids-rave-2.2.2/scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-21 13:30:33.000000 acids-rave-2.2.2/scripts/remote_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-21 13:30:33.000000 acids-rave-2.2.2/scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:35:21.964094 acids-rave-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 13:30:33.000000 acids-rave-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:35:21.964094 acids-rave-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:30:33.000000 acids-rave-2.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-21 13:30:33.000000 acids-rave-2.2.2/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-21 13:30:33.000000 acids-rave-2.2.2/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-21 13:30:33.000000 acids-rave-2.2.2/tests/test_residual.py
```

### Comparing `acids-rave-2.2.1/LICENSE` & `acids-rave-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/PKG-INFO` & `acids-rave-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-rave
-Version: 2.2.1
+Version: 2.2.2
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
-Metadata-Version: 2.1 Name: acids-rave Version: 2.2.1 Summary: RAVE: a Realtime
+Metadata-Version: 2.1 Name: acids-rave Version: 2.2.2 Summary: RAVE: a Realtime
 Audio Variatione autoEncoder Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE ![rave_logo](docs/rave.png) # RAVE: Realtime Audio
 Variational autoEncoder Official implementation of _RAVE: A variational
 autoencoder for fast and high-quality neural audio synthesis_ ([article link]
```

### Comparing `acids-rave-2.2.1/README.md` & `acids-rave-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/acids_rave.egg-info/PKG-INFO` & `acids-rave-2.2.2/acids_rave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-rave
-Version: 2.2.1
+Version: 2.2.2
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
-Metadata-Version: 2.1 Name: acids-rave Version: 2.2.1 Summary: RAVE: a Realtime
+Metadata-Version: 2.1 Name: acids-rave Version: 2.2.2 Summary: RAVE: a Realtime
 Audio Variatione autoEncoder Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE ![rave_logo](docs/rave.png) # RAVE: Realtime Audio
 Variational autoEncoder Official implementation of _RAVE: A variational
 autoencoder for fast and high-quality neural audio synthesis_ ([article link]
```

### Comparing `acids-rave-2.2.1/acids_rave.egg-info/SOURCES.txt` & `acids-rave-2.2.2/acids_rave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/__init__.py` & `acids-rave-2.2.2/rave/__init__.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/blocks.py` & `acids-rave-2.2.2/rave/blocks.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/configs/discrete.gin` & `acids-rave-2.2.2/rave/configs/discrete.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/configs/hybrid.gin` & `acids-rave-2.2.2/rave/configs/hybrid.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/configs/v1.gin` & `acids-rave-2.2.2/rave/configs/v1.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/configs/v2.gin` & `acids-rave-2.2.2/rave/configs/v2.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/configs/wasserstein.gin` & `acids-rave-2.2.2/rave/configs/wasserstein.gin`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/core.py` & `acids-rave-2.2.2/rave/core.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/dataset.py` & `acids-rave-2.2.2/rave/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/descript_discriminator.py` & `acids-rave-2.2.2/rave/descript_discriminator.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/discriminator.py` & `acids-rave-2.2.2/rave/discriminator.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/model.py` & `acids-rave-2.2.2/rave/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 from time import time
-from typing import Callable, Optional, Dict
+from typing import Callable, Dict, Optional
 
 import gin
 import numpy as np
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
 from einops import rearrange
```

### Comparing `acids-rave-2.2.1/rave/pqmf.py` & `acids-rave-2.2.2/rave/pqmf.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/quantization.py` & `acids-rave-2.2.2/rave/quantization.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/rave/resampler.py` & `acids-rave-2.2.2/rave/resampler.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/scripts/export.py` & `acids-rave-2.2.2/scripts/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     lower_bound=.1,
     upper_bound=.999,
     help='Fidelity to use during inference (Variational mode only)')
 flags.DEFINE_bool(
     'stereo',
     default=False,
     help='Enable fake stereo mode (one encoding, double decoding')
+flags.DEFINE_bool('ema_weights',
+                  default=False,
+                  help='Use ema weights if avaiable')
 flags.DEFINE_integer('sr',
                      default=None,
                      help='Optional resampling sample rate')
 
 
 class ScriptedRAVE(nn_tilde.Module):
 
@@ -120,14 +123,16 @@
 
         z = self.encoder(x_m)
 
         ratio_encode = x_len // z.shape[-1]
 
         channels = ["(L)", "(R)"] if stereo else ["(mono)"]
 
+        self.fake_adain = rave.blocks.AdaptiveInstanceNormalization(0)
+
         self.register_method(
             "encode",
             in_channels=1,
             in_ratio=1,
             out_channels=self.latent_size,
             out_ratio=ratio_encode,
             input_labels=['(signal) Input audio signal'],
@@ -333,18 +338,25 @@
     logging.info("building rave")
 
     gin.parse_config_file(os.path.join(FLAGS.run, "config.gin"))
     checkpoint = rave.core.search_for_run(FLAGS.run)
 
     pretrained = rave.RAVE()
     if checkpoint is not None:
-        pretrained.load_state_dict(
-            torch.load(checkpoint, map_location='cpu')["state_dict"],
-            strict=False,
-        )
+        checkpoint = torch.load(checkpoint, map_location='cpu')
+        if FLAGS.ema_weights and "EMA" in checkpoint["callbacks"]:
+            pretrained.load_state_dict(
+                checkpoint["callbacks"]["EMA"],
+                strict=False,
+            )
+        else:
+            pretrained.load_state_dict(
+                checkpoint["state_dict"],
+                strict=False,
+            )
     else:
         print("No checkpoint found, RAVE will remain randomly initialized")
     pretrained.eval()
 
     if isinstance(pretrained.encoder, rave.blocks.VariationalEncoder):
         script_class = VariationalScriptedRAVE
     elif isinstance(pretrained.encoder, rave.blocks.DiscreteEncoder):
```

### Comparing `acids-rave-2.2.1/scripts/export_onnx.py` & `acids-rave-2.2.2/scripts/export_onnx.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/scripts/main_cli.py` & `acids-rave-2.2.2/scripts/main_cli.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/scripts/preprocess.py` & `acids-rave-2.2.2/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/scripts/remote_dataset.py` & `acids-rave-2.2.2/scripts/remote_dataset.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/setup.py` & `acids-rave-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/tests/test_configs.py` & `acids-rave-2.2.2/tests/test_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import itertools
+import os
+import tempfile
 
 import gin
 import pytest
 import torch
 import torch.nn as nn
 
 import rave
@@ -91,7 +93,12 @@
     )
 
     scripted_rave_resampled = script_class(
         pretrained=model,
         stereo=stereo,
         target_sr=44100,
     )
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        scripted_rave.export_to_ts(os.path.join(tmpdir, "ori.ts"))
+        scripted_rave_resampled.export_to_ts(
+            os.path.join(tmpdir, "resampled.ts"))
```

### Comparing `acids-rave-2.2.1/tests/test_resampler.py` & `acids-rave-2.2.2/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `acids-rave-2.2.1/tests/test_residual.py` & `acids-rave-2.2.2/tests/test_residual.py`

 * *Files identical despite different names*

