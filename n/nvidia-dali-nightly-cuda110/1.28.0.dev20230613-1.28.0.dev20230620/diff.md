# Comparing `tmp/nvidia-dali-nightly-cuda110-1.28.0.dev20230613.tar.gz` & `tmp/nvidia-dali-nightly-cuda110-1.28.0.dev20230620.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda110-1.28.0.dev20230613.tar", last modified: Wed Jun 14 14:44:43 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda110-1.28.0.dev20230620.tar", last modified: Wed Jun 21 16:05:02 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230613.tar` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230620.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:44:43.078641 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-14 14:44:43.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-14 14:44:43.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-14 14:44:43.074640 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-14 14:44:43.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:44:43.074640 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/nvidia_dali_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-14 14:44:43.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-14 14:44:43.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-14 14:44:43.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-14 14:44:43.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-14 14:44:43.078641 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230613/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-21 16:05:02.626480 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-21 16:05:02.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 10:03:35.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-21 16:05:02.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-21 16:05:02.625480 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-21 16:05:02.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-21 16:05:02.625480 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-21 16:05:02.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-21 16:05:02.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-21 16:05:02.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-21 16:05:02.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-21 16:05:02.626480 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 10:03:35.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230620/setup.py
```

### Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230613/LICENSE.md` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230620/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230613/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230620/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.28.0.dev20230613
+Version: 1.28.0.dev20230620
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230613/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.28.0.dev20230613
+Version: 1.28.0.dev20230620
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230613/setup.py` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230620/setup.py`

 * *Files identical despite different names*

