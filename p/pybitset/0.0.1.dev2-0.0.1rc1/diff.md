# Comparing `tmp/pybitset-0.0.1.dev2.tar.gz` & `tmp/pybitset-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybitset-0.0.1.dev2.tar", last modified: Tue Jun 20 18:21:42 2023, max compression
+gzip compressed data, was "pybitset-0.0.1rc1.tar", last modified: Wed Jun 21 02:24:53 2023, max compression
```

## Comparing `pybitset-0.0.1.dev2.tar` & `pybitset-0.0.1rc1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/README.markdown
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.237546 pybitset-0.0.1.dev2/cbitset/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/msys2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/ubuntu18.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/ubuntu20.yml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-arm-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-clang-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-ninja-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/benchmarks/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/benchmarks/benchmark.c
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/benchmarks/lemirebenchmark.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/include/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/include/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/include/bitset.h
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/include/portability.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/src/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/src/bitset.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/tests/unit.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/pybitset/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/pybitset/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/pybitset/backends/cffi/
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cffi/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/pybitset/backends/cython/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   389578 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cython/_bitset.c
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cython/_bitset.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cython/bitset.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/pybitset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/README.markdown
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.112598 pybitset-0.0.1rc1/cbitset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.112598 pybitset-0.0.1rc1/cbitset/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.112598 pybitset-0.0.1rc1/cbitset/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.github/workflows/msys2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.github/workflows/ubuntu18.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.github/workflows/ubuntu20.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.github/workflows/vs16-arm-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.github/workflows/vs16-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.github/workflows/vs16-clang-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.github/workflows/vs16-ninja-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.112598 pybitset-0.0.1rc1/cbitset/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/benchmarks/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/benchmarks/benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/benchmarks/lemirebenchmark.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.112598 pybitset-0.0.1rc1/cbitset/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/include/bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/include/portability.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/cbitset/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/src/bitset.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/cbitset/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/cbitset/tests/unit.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/pybitset/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/pybitset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/pybitset/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/pybitset/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/pybitset/backends/cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/pybitset/backends/cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/pybitset/backends/cffi/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/pybitset/backends/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/pybitset/backends/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   390132 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/pybitset/backends/cython/_bitset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/pybitset/backends/cython/_bitset.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/pybitset/backends/cython/bitset.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/pybitset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-21 02:24:53.000000 pybitset-0.0.1rc1/pybitset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 02:24:53.000000 pybitset-0.0.1rc1/pybitset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 02:24:53.000000 pybitset-0.0.1rc1/pybitset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 02:24:53.000000 pybitset-0.0.1rc1/pybitset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 02:24:53.000000 pybitset-0.0.1rc1/pybitset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 02:24:53.000000 pybitset-0.0.1rc1/pybitset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 02:24:53.116598 pybitset-0.0.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-21 02:24:37.000000 pybitset-0.0.1rc1/setup.py
```

### Comparing `pybitset-0.0.1.dev2/PKG-INFO` & `pybitset-0.0.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybitset
-Version: 0.0.1.dev2
+Version: 0.0.1rc1
 Summary: python binding for cbitset
 Home-page: https://github.com/synodriver/pybitset
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: BSD
 Keywords: bitset
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pybitset-0.0.1.dev2/README.markdown` & `pybitset-0.0.1rc1/README.markdown`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/.github/workflows/msys2.yml` & `pybitset-0.0.1rc1/cbitset/.github/workflows/msys2.yml`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/.github/workflows/ubuntu18.yml` & `pybitset-0.0.1rc1/cbitset/.github/workflows/ubuntu18.yml`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/.github/workflows/ubuntu20.yml` & `pybitset-0.0.1rc1/cbitset/.github/workflows/ubuntu20.yml`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-ci.yml` & `pybitset-0.0.1rc1/cbitset/.github/workflows/vs16-ci.yml`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-clang-ci.yml` & `pybitset-0.0.1rc1/cbitset/.github/workflows/vs16-clang-ci.yml`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-ninja-ci.yml` & `pybitset-0.0.1rc1/cbitset/.github/workflows/vs16-ninja-ci.yml`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/LICENSE` & `pybitset-0.0.1rc1/cbitset/LICENSE`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/Makefile` & `pybitset-0.0.1rc1/cbitset/Makefile`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/README.md` & `pybitset-0.0.1rc1/cbitset/README.md`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/benchmarks/benchmark.c` & `pybitset-0.0.1rc1/cbitset/benchmarks/benchmark.c`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/benchmarks/lemirebenchmark.c` & `pybitset-0.0.1rc1/cbitset/benchmarks/lemirebenchmark.c`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/include/bitset.h` & `pybitset-0.0.1rc1/cbitset/include/bitset.h`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/include/portability.h` & `pybitset-0.0.1rc1/cbitset/include/portability.h`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/src/bitset.c` & `pybitset-0.0.1rc1/cbitset/src/bitset.c`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/cbitset/tests/unit.c` & `pybitset-0.0.1rc1/cbitset/tests/unit.c`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/pybitset/backends/cffi/__init__.py` & `pybitset-0.0.1rc1/pybitset/backends/cffi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
                 self._bitset = lib.bitset_create_with_capacity(size)
             if not self._bitset:
                 raise MemoryError
         else:
             self._bitset = ffi.NULL
 
     def __del__(self):
-        lib.bitset_free(self._bitset)
+        if self._bitset:
+            lib.bitset_free(self._bitset)
         self._bitset = ffi.NULL
 
     @staticmethod
     def from_ptr(ptr) -> "BitSet":
         self = BitSet(_init=False)
         self._bitset = ptr
         return self
```

### Comparing `pybitset-0.0.1.dev2/pybitset/backends/cffi/build.py` & `pybitset-0.0.1rc1/pybitset/backends/cffi/build.py`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/pybitset/backends/cython/_bitset.c` & `pybitset-0.0.1rc1/pybitset/backends/cython/_bitset.c`

 * *Files 0% similar despite different names*

```diff
@@ -1004,15 +1004,15 @@
 struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet {
   PyObject_HEAD
   struct __pyx_vtabstruct_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_vtab;
   bitset_t *_bitset;
 };
 
 
-/* "pybitset/backends/cython/_bitset.pyx":217
+/* "pybitset/backends/cython/_bitset.pyx":218
  * @cython.final
  * @cython.no_gc
  * cdef class BitSetIter:             # <<<<<<<<<<<<<<
  *     cdef:
  *         BitSet b
  */
 struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter {
@@ -1840,16 +1840,16 @@
   return __pyx_r;
 }
 
 /* "pybitset/backends/cython/_bitset.pyx":38
  *             self._bitset = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
- *         bitset_free(self._bitset)
- *         self._bitset = NULL
+ *         if self._bitset:
+ *             bitset_free(self._bitset)
  */
 
 /* Python wrapper */
 static void __pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
@@ -1857,47 +1857,67 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_2__dealloc__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "pybitset/backends/cython/_bitset.pyx":39
  * 
  *     def __dealloc__(self):
- *         bitset_free(self._bitset)             # <<<<<<<<<<<<<<
+ *         if self._bitset:             # <<<<<<<<<<<<<<
+ *             bitset_free(self._bitset)
+ *         self._bitset = NULL
+ */
+  __pyx_t_1 = (__pyx_v_self->_bitset != 0);
+  if (__pyx_t_1) {
+
+    /* "pybitset/backends/cython/_bitset.pyx":40
+ *     def __dealloc__(self):
+ *         if self._bitset:
+ *             bitset_free(self._bitset)             # <<<<<<<<<<<<<<
  *         self._bitset = NULL
  * 
  */
-  bitset_free(__pyx_v_self->_bitset);
+    bitset_free(__pyx_v_self->_bitset);
 
-  /* "pybitset/backends/cython/_bitset.pyx":40
+    /* "pybitset/backends/cython/_bitset.pyx":39
+ * 
  *     def __dealloc__(self):
- *         bitset_free(self._bitset)
+ *         if self._bitset:             # <<<<<<<<<<<<<<
+ *             bitset_free(self._bitset)
+ *         self._bitset = NULL
+ */
+  }
+
+  /* "pybitset/backends/cython/_bitset.pyx":41
+ *         if self._bitset:
+ *             bitset_free(self._bitset)
  *         self._bitset = NULL             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __pyx_v_self->_bitset = NULL;
 
   /* "pybitset/backends/cython/_bitset.pyx":38
  *             self._bitset = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
- *         bitset_free(self._bitset)
- *         self._bitset = NULL
+ *         if self._bitset:
+ *             bitset_free(self._bitset)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":43
+/* "pybitset/backends/cython/_bitset.pyx":44
  * 
  *     @staticmethod
  *     cdef inline BitSet from_ptr(bitset_t * ptr):             # <<<<<<<<<<<<<<
  *         cdef BitSet self = BitSet(_init=False)
  *         self._bitset = ptr
  */
 
@@ -1908,52 +1928,52 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("from_ptr", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":44
+  /* "pybitset/backends/cython/_bitset.pyx":45
  *     @staticmethod
  *     cdef inline BitSet from_ptr(bitset_t * ptr):
  *         cdef BitSet self = BitSet(_init=False)             # <<<<<<<<<<<<<<
  *         self._bitset = ptr
  *         return self
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_init, Py_False) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_init, Py_False) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self = ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":45
+  /* "pybitset/backends/cython/_bitset.pyx":46
  *     cdef inline BitSet from_ptr(bitset_t * ptr):
  *         cdef BitSet self = BitSet(_init=False)
  *         self._bitset = ptr             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->_bitset = __pyx_v_ptr;
 
-  /* "pybitset/backends/cython/_bitset.pyx":46
+  /* "pybitset/backends/cython/_bitset.pyx":47
  *         cdef BitSet self = BitSet(_init=False)
  *         self._bitset = ptr
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline clear(self):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = __pyx_v_self;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":43
+  /* "pybitset/backends/cython/_bitset.pyx":44
  * 
  *     @staticmethod
  *     cdef inline BitSet from_ptr(bitset_t * ptr):             # <<<<<<<<<<<<<<
  *         cdef BitSet self = BitSet(_init=False)
  *         self._bitset = ptr
  */
 
@@ -1966,54 +1986,54 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_self);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":48
+/* "pybitset/backends/cython/_bitset.pyx":49
  *         return self
  * 
  *     cpdef inline clear(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_clear(self._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_5clear(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_clear(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("clear", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":49
+  /* "pybitset/backends/cython/_bitset.pyx":50
  * 
  *     cpdef inline clear(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_clear(self._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":50
+        /* "pybitset/backends/cython/_bitset.pyx":51
  *     cpdef inline clear(self):
  *         with nogil:
  *             bitset_clear(self._bitset)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline fill(self):
  */
         bitset_clear(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":49
+      /* "pybitset/backends/cython/_bitset.pyx":50
  * 
  *     cpdef inline clear(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_clear(self._bitset)
  * 
  */
       /*finally:*/ {
@@ -2024,15 +2044,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":48
+  /* "pybitset/backends/cython/_bitset.pyx":49
  *         return self
  * 
  *     cpdef inline clear(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_clear(self._bitset)
  */
 
@@ -2062,15 +2082,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_clear(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_clear(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2079,54 +2099,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":52
+/* "pybitset/backends/cython/_bitset.pyx":53
  *             bitset_clear(self._bitset)
  * 
  *     cpdef inline fill(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_fill(self._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_7fill(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_fill(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("fill", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":53
+  /* "pybitset/backends/cython/_bitset.pyx":54
  * 
  *     cpdef inline fill(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_fill(self._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":54
+        /* "pybitset/backends/cython/_bitset.pyx":55
  *     cpdef inline fill(self):
  *         with nogil:
  *             bitset_fill(self._bitset)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline BitSet copy(self):
  */
         bitset_fill(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":53
+      /* "pybitset/backends/cython/_bitset.pyx":54
  * 
  *     cpdef inline fill(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_fill(self._bitset)
  * 
  */
       /*finally:*/ {
@@ -2137,15 +2157,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":52
+  /* "pybitset/backends/cython/_bitset.pyx":53
  *             bitset_clear(self._bitset)
  * 
  *     cpdef inline fill(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_fill(self._bitset)
  */
 
@@ -2175,15 +2195,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fill", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_fill(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_fill(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2192,15 +2212,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":56
+/* "pybitset/backends/cython/_bitset.pyx":57
  *             bitset_fill(self._bitset)
  * 
  *     cpdef inline BitSet copy(self):             # <<<<<<<<<<<<<<
  *         cdef bitset_t *ret
  *         with nogil:
  */
 
@@ -2211,40 +2231,40 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":58
+  /* "pybitset/backends/cython/_bitset.pyx":59
  *     cpdef inline BitSet copy(self):
  *         cdef bitset_t *ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_copy(self._bitset)
  *         return BitSet.from_ptr(ret)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":59
+        /* "pybitset/backends/cython/_bitset.pyx":60
  *         cdef bitset_t *ret
  *         with nogil:
  *             ret = bitset_copy(self._bitset)             # <<<<<<<<<<<<<<
  *         return BitSet.from_ptr(ret)
  * 
  */
         __pyx_v_ret = bitset_copy(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":58
+      /* "pybitset/backends/cython/_bitset.pyx":59
  *     cpdef inline BitSet copy(self):
  *         cdef bitset_t *ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_copy(self._bitset)
  *         return BitSet.from_ptr(ret)
  */
       /*finally:*/ {
@@ -2255,29 +2275,29 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":60
+  /* "pybitset/backends/cython/_bitset.pyx":61
  *         with nogil:
  *             ret = bitset_copy(self._bitset)
  *         return BitSet.from_ptr(ret)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __pyx_t_1 = ((PyObject *)__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_from_ptr(__pyx_v_ret)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_from_ptr(__pyx_v_ret)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":56
+  /* "pybitset/backends/cython/_bitset.pyx":57
  *             bitset_fill(self._bitset)
  * 
  *     cpdef inline BitSet copy(self):             # <<<<<<<<<<<<<<
  *         cdef bitset_t *ret
  *         with nogil:
  */
 
@@ -2311,15 +2331,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_copy(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_copy(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2328,55 +2348,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":62
+/* "pybitset/backends/cython/_bitset.pyx":63
  *         return BitSet.from_ptr(ret)
  * 
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_11resize(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_resize(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_newarraysize, int __pyx_v_padwithzeroes, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("resize", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":64
+  /* "pybitset/backends/cython/_bitset.pyx":65
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":65
+        /* "pybitset/backends/cython/_bitset.pyx":66
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_resize(__pyx_v_self->_bitset, __pyx_v_newarraysize, __pyx_v_padwithzeroes);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":64
+      /* "pybitset/backends/cython/_bitset.pyx":65
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)
  *         return ret
  */
       /*finally:*/ {
@@ -2387,25 +2407,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":66
+  /* "pybitset/backends/cython/_bitset.pyx":67
  *         with nogil:
  *             ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t size_in_bytes(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":62
+  /* "pybitset/backends/cython/_bitset.pyx":63
  *         return BitSet.from_ptr(ret)
  * 
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -2446,32 +2466,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_newarraysize)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_padwithzeroes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("resize", 1, 2, 2, 1); __PYX_ERR(0, 62, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("resize", 1, 2, 2, 1); __PYX_ERR(0, 63, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resize") < 0)) __PYX_ERR(0, 62, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resize") < 0)) __PYX_ERR(0, 63, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_newarraysize = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_newarraysize == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
-    __pyx_v_padwithzeroes = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_padwithzeroes == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
+    __pyx_v_newarraysize = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_newarraysize == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 63, __pyx_L3_error)
+    __pyx_v_padwithzeroes = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_padwithzeroes == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 63, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("resize", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 62, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("resize", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 63, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.resize", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_10resize(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), __pyx_v_newarraysize, __pyx_v_padwithzeroes);
 
@@ -2485,15 +2505,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("resize", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_resize(__pyx_v_self, __pyx_v_newarraysize, __pyx_v_padwithzeroes, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_resize(__pyx_v_self, __pyx_v_newarraysize, __pyx_v_padwithzeroes, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2502,55 +2522,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":68
+/* "pybitset/backends/cython/_bitset.pyx":69
  *         return ret
  * 
  *     cpdef inline size_t size_in_bytes(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_13size_in_bytes(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bytes(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("size_in_bytes", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":70
+  /* "pybitset/backends/cython/_bitset.pyx":71
  *     cpdef inline size_t size_in_bytes(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_bytes(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":71
+        /* "pybitset/backends/cython/_bitset.pyx":72
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_size_in_bytes(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_size_in_bytes(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":70
+      /* "pybitset/backends/cython/_bitset.pyx":71
  *     cpdef inline size_t size_in_bytes(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_bytes(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -2561,25 +2581,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":72
+  /* "pybitset/backends/cython/_bitset.pyx":73
  *         with nogil:
  *             ret = bitset_size_in_bytes(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t size_in_bits(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":68
+  /* "pybitset/backends/cython/_bitset.pyx":69
  *         return ret
  * 
  *     cpdef inline size_t size_in_bytes(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -2608,15 +2628,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("size_in_bytes", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bytes(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bytes(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2625,55 +2645,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":74
+/* "pybitset/backends/cython/_bitset.pyx":75
  *         return ret
  * 
  *     cpdef inline size_t size_in_bits(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_15size_in_bits(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bits(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("size_in_bits", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":76
+  /* "pybitset/backends/cython/_bitset.pyx":77
  *     cpdef inline size_t size_in_bits(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_bits(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":77
+        /* "pybitset/backends/cython/_bitset.pyx":78
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_size_in_bits(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_size_in_bits(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":76
+      /* "pybitset/backends/cython/_bitset.pyx":77
  *     cpdef inline size_t size_in_bits(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_bits(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -2684,25 +2704,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":78
+  /* "pybitset/backends/cython/_bitset.pyx":79
  *         with nogil:
  *             ret = bitset_size_in_bits(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t size_in_words(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":74
+  /* "pybitset/backends/cython/_bitset.pyx":75
  *         return ret
  * 
  *     cpdef inline size_t size_in_bits(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -2731,15 +2751,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("size_in_bits", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bits(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bits(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2748,55 +2768,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":80
+/* "pybitset/backends/cython/_bitset.pyx":81
  *         return ret
  * 
  *     cpdef inline size_t size_in_words(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_17size_in_words(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_words(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("size_in_words", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":82
+  /* "pybitset/backends/cython/_bitset.pyx":83
  *     cpdef inline size_t size_in_words(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_words(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":83
+        /* "pybitset/backends/cython/_bitset.pyx":84
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_size_in_words(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_size_in_words(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":82
+      /* "pybitset/backends/cython/_bitset.pyx":83
  *     cpdef inline size_t size_in_words(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_words(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -2807,25 +2827,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":84
+  /* "pybitset/backends/cython/_bitset.pyx":85
  *         with nogil:
  *             ret = bitset_size_in_words(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint grow(self, size_t newarraysize):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":80
+  /* "pybitset/backends/cython/_bitset.pyx":81
  *         return ret
  * 
  *     cpdef inline size_t size_in_words(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -2854,15 +2874,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("size_in_words", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_words(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_words(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2871,55 +2891,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":86
+/* "pybitset/backends/cython/_bitset.pyx":87
  *         return ret
  * 
  *     cpdef inline bint grow(self, size_t newarraysize):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_19grow(PyObject *__pyx_v_self, PyObject *__pyx_arg_newarraysize); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_grow(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_newarraysize, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("grow", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":88
+  /* "pybitset/backends/cython/_bitset.pyx":89
  *     cpdef inline bint grow(self, size_t newarraysize):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_grow(self._bitset, newarraysize)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":89
+        /* "pybitset/backends/cython/_bitset.pyx":90
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_grow(self._bitset, newarraysize)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_grow(__pyx_v_self->_bitset, __pyx_v_newarraysize);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":88
+      /* "pybitset/backends/cython/_bitset.pyx":89
  *     cpdef inline bint grow(self, size_t newarraysize):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_grow(self._bitset, newarraysize)
  *         return ret
  */
       /*finally:*/ {
@@ -2930,25 +2950,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":90
+  /* "pybitset/backends/cython/_bitset.pyx":91
  *         with nogil:
  *             ret = bitset_grow(self._bitset, newarraysize)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint trim(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":86
+  /* "pybitset/backends/cython/_bitset.pyx":87
  *         return ret
  * 
  *     cpdef inline bint grow(self, size_t newarraysize):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -2966,15 +2986,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("grow (wrapper)", 0);
   assert(__pyx_arg_newarraysize); {
-    __pyx_v_newarraysize = __Pyx_PyInt_As_size_t(__pyx_arg_newarraysize); if (unlikely((__pyx_v_newarraysize == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
+    __pyx_v_newarraysize = __Pyx_PyInt_As_size_t(__pyx_arg_newarraysize); if (unlikely((__pyx_v_newarraysize == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 87, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.grow", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -2990,15 +3010,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("grow", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_grow(__pyx_v_self, __pyx_v_newarraysize, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_grow(__pyx_v_self, __pyx_v_newarraysize, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3007,55 +3027,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":92
+/* "pybitset/backends/cython/_bitset.pyx":93
  *         return ret
  * 
  *     cpdef inline bint trim(self):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_21trim(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_trim(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("trim", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":94
+  /* "pybitset/backends/cython/_bitset.pyx":95
  *     cpdef inline bint trim(self):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_trim(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":95
+        /* "pybitset/backends/cython/_bitset.pyx":96
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_trim(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_trim(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":94
+      /* "pybitset/backends/cython/_bitset.pyx":95
  *     cpdef inline bint trim(self):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_trim(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -3066,25 +3086,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":96
+  /* "pybitset/backends/cython/_bitset.pyx":97
  *         with nogil:
  *             ret = bitset_trim(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline shift_left(self, size_t s):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":92
+  /* "pybitset/backends/cython/_bitset.pyx":93
  *         return ret
  * 
  *     cpdef inline bint trim(self):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -3113,15 +3133,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("trim", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_trim(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_trim(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3130,54 +3150,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":98
+/* "pybitset/backends/cython/_bitset.pyx":99
  *         return ret
  * 
  *     cpdef inline shift_left(self, size_t s):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_shift_left(self._bitset, s)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_23shift_left(PyObject *__pyx_v_self, PyObject *__pyx_arg_s); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_left(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_s, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shift_left", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":99
+  /* "pybitset/backends/cython/_bitset.pyx":100
  * 
  *     cpdef inline shift_left(self, size_t s):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_shift_left(self._bitset, s)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":100
+        /* "pybitset/backends/cython/_bitset.pyx":101
  *     cpdef inline shift_left(self, size_t s):
  *         with nogil:
  *             bitset_shift_left(self._bitset, s)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline shift_right(self, size_t s):
  */
         bitset_shift_left(__pyx_v_self->_bitset, __pyx_v_s);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":99
+      /* "pybitset/backends/cython/_bitset.pyx":100
  * 
  *     cpdef inline shift_left(self, size_t s):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_shift_left(self._bitset, s)
  * 
  */
       /*finally:*/ {
@@ -3188,15 +3208,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":98
+  /* "pybitset/backends/cython/_bitset.pyx":99
  *         return ret
  * 
  *     cpdef inline shift_left(self, size_t s):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_shift_left(self._bitset, s)
  */
 
@@ -3215,15 +3235,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shift_left (wrapper)", 0);
   assert(__pyx_arg_s); {
-    __pyx_v_s = __Pyx_PyInt_As_size_t(__pyx_arg_s); if (unlikely((__pyx_v_s == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L3_error)
+    __pyx_v_s = __Pyx_PyInt_As_size_t(__pyx_arg_s); if (unlikely((__pyx_v_s == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.shift_left", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3239,15 +3259,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shift_left", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_left(__pyx_v_self, __pyx_v_s, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_left(__pyx_v_self, __pyx_v_s, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3256,54 +3276,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":102
+/* "pybitset/backends/cython/_bitset.pyx":103
  *             bitset_shift_left(self._bitset, s)
  * 
  *     cpdef inline shift_right(self, size_t s):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_shift_right(self._bitset, s)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_25shift_right(PyObject *__pyx_v_self, PyObject *__pyx_arg_s); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_right(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_s, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shift_right", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":103
+  /* "pybitset/backends/cython/_bitset.pyx":104
  * 
  *     cpdef inline shift_right(self, size_t s):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_shift_right(self._bitset, s)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":104
+        /* "pybitset/backends/cython/_bitset.pyx":105
  *     cpdef inline shift_right(self, size_t s):
  *         with nogil:
  *             bitset_shift_right(self._bitset, s)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline set(self,  size_t i):
  */
         bitset_shift_right(__pyx_v_self->_bitset, __pyx_v_s);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":103
+      /* "pybitset/backends/cython/_bitset.pyx":104
  * 
  *     cpdef inline shift_right(self, size_t s):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_shift_right(self._bitset, s)
  * 
  */
       /*finally:*/ {
@@ -3314,15 +3334,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":102
+  /* "pybitset/backends/cython/_bitset.pyx":103
  *             bitset_shift_left(self._bitset, s)
  * 
  *     cpdef inline shift_right(self, size_t s):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_shift_right(self._bitset, s)
  */
 
@@ -3341,15 +3361,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shift_right (wrapper)", 0);
   assert(__pyx_arg_s); {
-    __pyx_v_s = __Pyx_PyInt_As_size_t(__pyx_arg_s); if (unlikely((__pyx_v_s == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 102, __pyx_L3_error)
+    __pyx_v_s = __Pyx_PyInt_As_size_t(__pyx_arg_s); if (unlikely((__pyx_v_s == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.shift_right", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3365,15 +3385,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shift_right", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_right(__pyx_v_self, __pyx_v_s, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_right(__pyx_v_self, __pyx_v_s, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3382,54 +3402,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":106
+/* "pybitset/backends/cython/_bitset.pyx":107
  *             bitset_shift_right(self._bitset, s)
  * 
  *     cpdef inline set(self,  size_t i):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_set(self._bitset, i)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_27set(PyObject *__pyx_v_self, PyObject *__pyx_arg_i); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_i, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":107
+  /* "pybitset/backends/cython/_bitset.pyx":108
  * 
  *     cpdef inline set(self,  size_t i):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_set(self._bitset, i)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":108
+        /* "pybitset/backends/cython/_bitset.pyx":109
  *     cpdef inline set(self,  size_t i):
  *         with nogil:
  *             bitset_set(self._bitset, i)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):
  */
         bitset_set(__pyx_v_self->_bitset, __pyx_v_i);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":107
+      /* "pybitset/backends/cython/_bitset.pyx":108
  * 
  *     cpdef inline set(self,  size_t i):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_set(self._bitset, i)
  * 
  */
       /*finally:*/ {
@@ -3440,15 +3460,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":106
+  /* "pybitset/backends/cython/_bitset.pyx":107
  *             bitset_shift_right(self._bitset, s)
  * 
  *     cpdef inline set(self,  size_t i):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_set(self._bitset, i)
  */
 
@@ -3467,15 +3487,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set (wrapper)", 0);
   assert(__pyx_arg_i); {
-    __pyx_v_i = __Pyx_PyInt_As_size_t(__pyx_arg_i); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L3_error)
+    __pyx_v_i = __Pyx_PyInt_As_size_t(__pyx_arg_i); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.set", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3491,15 +3511,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set(__pyx_v_self, __pyx_v_i, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set(__pyx_v_self, __pyx_v_i, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3508,54 +3528,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":110
+/* "pybitset/backends/cython/_bitset.pyx":111
  *             bitset_set(self._bitset, i)
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_set_to_value(self._bitset, i, flag)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_29set_to_value(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set_to_value(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_i, int __pyx_v_flag, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_to_value", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":111
+  /* "pybitset/backends/cython/_bitset.pyx":112
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_set_to_value(self._bitset, i, flag)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":112
+        /* "pybitset/backends/cython/_bitset.pyx":113
  *     cpdef inline set_to_value(self, size_t i, bint flag):
  *         with nogil:
  *             bitset_set_to_value(self._bitset, i, flag)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint get(self, size_t i):
  */
         bitset_set_to_value(__pyx_v_self->_bitset, __pyx_v_i, __pyx_v_flag);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":111
+      /* "pybitset/backends/cython/_bitset.pyx":112
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_set_to_value(self._bitset, i, flag)
  * 
  */
       /*finally:*/ {
@@ -3566,15 +3586,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":110
+  /* "pybitset/backends/cython/_bitset.pyx":111
  *             bitset_set(self._bitset, i)
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_set_to_value(self._bitset, i, flag)
  */
 
@@ -3616,32 +3636,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_i)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flag)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_to_value", 1, 2, 2, 1); __PYX_ERR(0, 110, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_to_value", 1, 2, 2, 1); __PYX_ERR(0, 111, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_to_value") < 0)) __PYX_ERR(0, 110, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_to_value") < 0)) __PYX_ERR(0, 111, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_i = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
-    __pyx_v_flag = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_flag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
+    __pyx_v_i = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L3_error)
+    __pyx_v_flag = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_flag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_to_value", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 110, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_to_value", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 111, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.set_to_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_28set_to_value(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), __pyx_v_i, __pyx_v_flag);
 
@@ -3655,15 +3675,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_to_value", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set_to_value(__pyx_v_self, __pyx_v_i, __pyx_v_flag, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set_to_value(__pyx_v_self, __pyx_v_i, __pyx_v_flag, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3672,55 +3692,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":114
+/* "pybitset/backends/cython/_bitset.pyx":115
  *             bitset_set_to_value(self._bitset, i, flag)
  * 
  *     cpdef inline bint get(self, size_t i):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_31get(PyObject *__pyx_v_self, PyObject *__pyx_arg_i); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_get(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_i, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":116
+  /* "pybitset/backends/cython/_bitset.pyx":117
  *     cpdef inline bint get(self, size_t i):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_get(self._bitset, i)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":117
+        /* "pybitset/backends/cython/_bitset.pyx":118
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_get(self._bitset, i)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_get(__pyx_v_self->_bitset, __pyx_v_i);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":116
+      /* "pybitset/backends/cython/_bitset.pyx":117
  *     cpdef inline bint get(self, size_t i):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_get(self._bitset, i)
  *         return ret
  */
       /*finally:*/ {
@@ -3731,25 +3751,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":118
+  /* "pybitset/backends/cython/_bitset.pyx":119
  *         with nogil:
  *             ret = bitset_get(self._bitset, i)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t count(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":114
+  /* "pybitset/backends/cython/_bitset.pyx":115
  *             bitset_set_to_value(self._bitset, i, flag)
  * 
  *     cpdef inline bint get(self, size_t i):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -3767,15 +3787,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get (wrapper)", 0);
   assert(__pyx_arg_i); {
-    __pyx_v_i = __Pyx_PyInt_As_size_t(__pyx_arg_i); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+    __pyx_v_i = __Pyx_PyInt_As_size_t(__pyx_arg_i); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3791,15 +3811,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_get(__pyx_v_self, __pyx_v_i, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_get(__pyx_v_self, __pyx_v_i, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3808,55 +3828,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":120
+/* "pybitset/backends/cython/_bitset.pyx":121
  *         return ret
  * 
  *     cpdef inline size_t count(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_33count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":122
+  /* "pybitset/backends/cython/_bitset.pyx":123
  *     cpdef inline size_t count(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_count(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":123
+        /* "pybitset/backends/cython/_bitset.pyx":124
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_count(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_count(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":122
+      /* "pybitset/backends/cython/_bitset.pyx":123
  *     cpdef inline size_t count(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_count(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -3867,25 +3887,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":124
+  /* "pybitset/backends/cython/_bitset.pyx":125
  *         with nogil:
  *             ret = bitset_count(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t minimum(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":120
+  /* "pybitset/backends/cython/_bitset.pyx":121
  *         return ret
  * 
  *     cpdef inline size_t count(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -3914,15 +3934,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_count(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_count(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3931,55 +3951,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":126
+/* "pybitset/backends/cython/_bitset.pyx":127
  *         return ret
  * 
  *     cpdef inline size_t minimum(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_35minimum(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_minimum(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("minimum", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":128
+  /* "pybitset/backends/cython/_bitset.pyx":129
  *     cpdef inline size_t minimum(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_minimum(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":129
+        /* "pybitset/backends/cython/_bitset.pyx":130
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_minimum(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_minimum(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":128
+      /* "pybitset/backends/cython/_bitset.pyx":129
  *     cpdef inline size_t minimum(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_minimum(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -3990,25 +4010,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":130
+  /* "pybitset/backends/cython/_bitset.pyx":131
  *         with nogil:
  *             ret = bitset_minimum(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t maximum(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":126
+  /* "pybitset/backends/cython/_bitset.pyx":127
  *         return ret
  * 
  *     cpdef inline size_t minimum(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -4037,15 +4057,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("minimum", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_minimum(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_minimum(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4054,55 +4074,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":132
+/* "pybitset/backends/cython/_bitset.pyx":133
  *         return ret
  * 
  *     cpdef inline size_t maximum(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_37maximum(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_maximum(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("maximum", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":134
+  /* "pybitset/backends/cython/_bitset.pyx":135
  *     cpdef inline size_t maximum(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_maximum(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":135
+        /* "pybitset/backends/cython/_bitset.pyx":136
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_maximum(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_maximum(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":134
+      /* "pybitset/backends/cython/_bitset.pyx":135
  *     cpdef inline size_t maximum(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_maximum(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4113,25 +4133,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":136
+  /* "pybitset/backends/cython/_bitset.pyx":137
  *         with nogil:
  *             ret = bitset_maximum(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint inplace_union(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":132
+  /* "pybitset/backends/cython/_bitset.pyx":133
  *         return ret
  * 
  *     cpdef inline size_t maximum(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -4160,15 +4180,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("maximum", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_maximum(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_maximum(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4177,55 +4197,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":138
+/* "pybitset/backends/cython/_bitset.pyx":139
  *         return ret
  * 
  *     cpdef inline bint inplace_union(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_39inplace_union(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_union(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_union", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":140
+  /* "pybitset/backends/cython/_bitset.pyx":141
  *     cpdef inline bint inplace_union(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_inplace_union(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":141
+        /* "pybitset/backends/cython/_bitset.pyx":142
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_inplace_union(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_inplace_union(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":140
+      /* "pybitset/backends/cython/_bitset.pyx":141
  *     cpdef inline bint inplace_union(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_inplace_union(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4236,25 +4256,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":142
+  /* "pybitset/backends/cython/_bitset.pyx":143
  *         with nogil:
  *             ret = bitset_inplace_union(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t union_count(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":138
+  /* "pybitset/backends/cython/_bitset.pyx":139
  *         return ret
  * 
  *     cpdef inline bint inplace_union(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -4270,15 +4290,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_39inplace_union(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_union (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 138, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 139, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_38inplace_union(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4291,15 +4311,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inplace_union", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_union(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_union(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4308,55 +4328,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":144
+/* "pybitset/backends/cython/_bitset.pyx":145
  *         return ret
  * 
  *     cpdef inline size_t union_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_41union_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_union_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("union_count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":146
+  /* "pybitset/backends/cython/_bitset.pyx":147
  *     cpdef inline size_t union_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_union_count(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":147
+        /* "pybitset/backends/cython/_bitset.pyx":148
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_union_count(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_union_count(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":146
+      /* "pybitset/backends/cython/_bitset.pyx":147
  *     cpdef inline size_t union_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_union_count(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4367,25 +4387,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":148
+  /* "pybitset/backends/cython/_bitset.pyx":149
  *         with nogil:
  *             ret = bitset_union_count(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":144
+  /* "pybitset/backends/cython/_bitset.pyx":145
  *         return ret
  * 
  *     cpdef inline size_t union_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -4401,15 +4421,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_41union_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("union_count (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 145, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_40union_count(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4422,15 +4442,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("union_count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_union_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_union_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4439,54 +4459,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":150
+/* "pybitset/backends/cython/_bitset.pyx":151
  *         return ret
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_43inplace_intersection(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_intersection(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_intersection", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":151
+  /* "pybitset/backends/cython/_bitset.pyx":152
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":152
+        /* "pybitset/backends/cython/_bitset.pyx":153
  *     cpdef inline inplace_intersection(self, BitSet b2):
  *         with nogil:
  *             bitset_inplace_intersection(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t intersection_count(self, BitSet b2):
  */
         bitset_inplace_intersection(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":151
+      /* "pybitset/backends/cython/_bitset.pyx":152
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  * 
  */
       /*finally:*/ {
@@ -4497,15 +4517,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":150
+  /* "pybitset/backends/cython/_bitset.pyx":151
  *         return ret
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  */
 
@@ -4522,15 +4542,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_43inplace_intersection(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_intersection (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 151, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_42inplace_intersection(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4543,15 +4563,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inplace_intersection", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_intersection(__pyx_v_self, __pyx_v_b2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_intersection(__pyx_v_self, __pyx_v_b2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4560,55 +4580,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":154
+/* "pybitset/backends/cython/_bitset.pyx":155
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  * 
  *     cpdef inline size_t intersection_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_45intersection_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersection_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersection_count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":156
+  /* "pybitset/backends/cython/_bitset.pyx":157
  *     cpdef inline size_t intersection_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_intersection_count(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":157
+        /* "pybitset/backends/cython/_bitset.pyx":158
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_intersection_count(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_intersection_count(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":156
+      /* "pybitset/backends/cython/_bitset.pyx":157
  *     cpdef inline size_t intersection_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_intersection_count(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4619,25 +4639,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":158
+  /* "pybitset/backends/cython/_bitset.pyx":159
  *         with nogil:
  *             ret = bitset_intersection_count(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint disjoint(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":154
+  /* "pybitset/backends/cython/_bitset.pyx":155
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  * 
  *     cpdef inline size_t intersection_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -4653,15 +4673,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_45intersection_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersection_count (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 155, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_44intersection_count(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4674,15 +4694,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("intersection_count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersection_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersection_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4691,55 +4711,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":160
+/* "pybitset/backends/cython/_bitset.pyx":161
  *         return ret
  * 
  *     cpdef inline bint disjoint(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_47disjoint(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_disjoint(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("disjoint", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":162
+  /* "pybitset/backends/cython/_bitset.pyx":163
  *     cpdef inline bint disjoint(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitsets_disjoint(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":163
+        /* "pybitset/backends/cython/_bitset.pyx":164
  *         cdef bint ret
  *         with nogil:
  *             ret = bitsets_disjoint(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitsets_disjoint(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":162
+      /* "pybitset/backends/cython/_bitset.pyx":163
  *     cpdef inline bint disjoint(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitsets_disjoint(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4750,25 +4770,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":164
+  /* "pybitset/backends/cython/_bitset.pyx":165
  *         with nogil:
  *             ret = bitsets_disjoint(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint intersect(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":160
+  /* "pybitset/backends/cython/_bitset.pyx":161
  *         return ret
  * 
  *     cpdef inline bint disjoint(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -4784,15 +4804,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_47disjoint(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("disjoint (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 161, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_46disjoint(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4805,15 +4825,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("disjoint", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_disjoint(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_disjoint(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4822,55 +4842,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":166
+/* "pybitset/backends/cython/_bitset.pyx":167
  *         return ret
  * 
  *     cpdef inline bint intersect(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_49intersect(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersect(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":168
+  /* "pybitset/backends/cython/_bitset.pyx":169
  *     cpdef inline bint intersect(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitsets_intersect(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":169
+        /* "pybitset/backends/cython/_bitset.pyx":170
  *         cdef bint ret
  *         with nogil:
  *             ret = bitsets_intersect(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitsets_intersect(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":168
+      /* "pybitset/backends/cython/_bitset.pyx":169
  *     cpdef inline bint intersect(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitsets_intersect(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4881,25 +4901,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":170
+  /* "pybitset/backends/cython/_bitset.pyx":171
  *         with nogil:
  *             ret = bitsets_intersect(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint contains_all(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":166
+  /* "pybitset/backends/cython/_bitset.pyx":167
  *         return ret
  * 
  *     cpdef inline bint intersect(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -4915,15 +4935,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_49intersect(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 167, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_48intersect(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4936,15 +4956,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("intersect", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersect(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersect(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4953,55 +4973,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":172
+/* "pybitset/backends/cython/_bitset.pyx":173
  *         return ret
  * 
  *     cpdef inline bint contains_all(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_51contains_all(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_contains_all(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("contains_all", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":174
+  /* "pybitset/backends/cython/_bitset.pyx":175
  *     cpdef inline bint contains_all(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_contains_all(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":175
+        /* "pybitset/backends/cython/_bitset.pyx":176
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_contains_all(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_contains_all(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":174
+      /* "pybitset/backends/cython/_bitset.pyx":175
  *     cpdef inline bint contains_all(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_contains_all(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -5012,25 +5032,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":176
+  /* "pybitset/backends/cython/_bitset.pyx":177
  *         with nogil:
  *             ret = bitset_contains_all(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":172
+  /* "pybitset/backends/cython/_bitset.pyx":173
  *         return ret
  * 
  *     cpdef inline bint contains_all(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -5046,15 +5066,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_51contains_all(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("contains_all (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 172, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 173, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_50contains_all(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5067,15 +5087,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("contains_all", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_contains_all(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_contains_all(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5084,54 +5104,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":178
+/* "pybitset/backends/cython/_bitset.pyx":179
  *         return ret
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_53inplace_difference(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_difference(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_difference", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":179
+  /* "pybitset/backends/cython/_bitset.pyx":180
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":180
+        /* "pybitset/backends/cython/_bitset.pyx":181
  *     cpdef inline inplace_difference(self, BitSet b2):
  *         with nogil:
  *             bitset_inplace_difference(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t difference_count(self, BitSet b2):
  */
         bitset_inplace_difference(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":179
+      /* "pybitset/backends/cython/_bitset.pyx":180
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  * 
  */
       /*finally:*/ {
@@ -5142,15 +5162,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":178
+  /* "pybitset/backends/cython/_bitset.pyx":179
  *         return ret
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  */
 
@@ -5167,15 +5187,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_53inplace_difference(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_difference (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 179, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_52inplace_difference(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5188,15 +5208,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inplace_difference", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_difference(__pyx_v_self, __pyx_v_b2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_difference(__pyx_v_self, __pyx_v_b2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5205,55 +5225,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":182
+/* "pybitset/backends/cython/_bitset.pyx":183
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  * 
  *     cpdef inline size_t difference_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_55difference_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_difference_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("difference_count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":184
+  /* "pybitset/backends/cython/_bitset.pyx":185
  *     cpdef inline size_t difference_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_difference_count(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":185
+        /* "pybitset/backends/cython/_bitset.pyx":186
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_difference_count(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_difference_count(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":184
+      /* "pybitset/backends/cython/_bitset.pyx":185
  *     cpdef inline size_t difference_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_difference_count(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -5264,25 +5284,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":186
+  /* "pybitset/backends/cython/_bitset.pyx":187
  *         with nogil:
  *             ret = bitset_difference_count(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":182
+  /* "pybitset/backends/cython/_bitset.pyx":183
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  * 
  *     cpdef inline size_t difference_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -5298,15 +5318,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_55difference_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("difference_count (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 182, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 183, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_54difference_count(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5319,15 +5339,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("difference_count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_difference_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_difference_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5336,55 +5356,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":188
+/* "pybitset/backends/cython/_bitset.pyx":189
  *         return ret
  * 
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_57inplace_symmetric_difference(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_symmetric_difference(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_symmetric_difference", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":190
+  /* "pybitset/backends/cython/_bitset.pyx":191
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":191
+        /* "pybitset/backends/cython/_bitset.pyx":192
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_inplace_symmetric_difference(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":190
+      /* "pybitset/backends/cython/_bitset.pyx":191
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -5395,25 +5415,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":192
+  /* "pybitset/backends/cython/_bitset.pyx":193
  *         with nogil:
  *             ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":188
+  /* "pybitset/backends/cython/_bitset.pyx":189
  *         return ret
  * 
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -5429,15 +5449,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_57inplace_symmetric_difference(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_symmetric_difference (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 189, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_56inplace_symmetric_difference(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5450,15 +5470,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inplace_symmetric_difference", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_symmetric_difference(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_symmetric_difference(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5467,55 +5487,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":194
+/* "pybitset/backends/cython/_bitset.pyx":195
  *         return ret
  * 
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_59symmetric_difference_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_symmetric_difference_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("symmetric_difference_count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":196
+  /* "pybitset/backends/cython/_bitset.pyx":197
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":197
+        /* "pybitset/backends/cython/_bitset.pyx":198
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_symmetric_difference_count(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":196
+      /* "pybitset/backends/cython/_bitset.pyx":197
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -5526,25 +5546,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":198
+  /* "pybitset/backends/cython/_bitset.pyx":199
  *         with nogil:
  *             ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":194
+  /* "pybitset/backends/cython/_bitset.pyx":195
  *         return ret
  * 
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -5560,15 +5580,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_59symmetric_difference_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("symmetric_difference_count (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 194, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 195, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_58symmetric_difference_count(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5581,15 +5601,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("symmetric_difference_count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_symmetric_difference_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_symmetric_difference_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5598,15 +5618,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":200
+/* "pybitset/backends/cython/_bitset.pyx":201
  *         return ret
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return BitSetIter(self)
  * 
  */
 
@@ -5628,29 +5648,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":201
+  /* "pybitset/backends/cython/_bitset.pyx":202
  * 
  *     def __iter__(self):
  *         return BitSetIter(self)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint for_each(self, object func):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSetIter), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSetIter), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":200
+  /* "pybitset/backends/cython/_bitset.pyx":201
  *         return ret
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return BitSetIter(self)
  * 
  */
 
@@ -5661,55 +5681,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":203
+/* "pybitset/backends/cython/_bitset.pyx":204
  *         return BitSetIter(self)
  * 
  *     cpdef inline bint for_each(self, object func):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_63for_each(PyObject *__pyx_v_self, PyObject *__pyx_v_func); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_for_each(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, PyObject *__pyx_v_func, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("for_each", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":205
+  /* "pybitset/backends/cython/_bitset.pyx":206
  *     cpdef inline bint for_each(self, object func):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":206
+        /* "pybitset/backends/cython/_bitset.pyx":207
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_for_each(__pyx_v_self->_bitset, __pyx_f_8pybitset_8backends_6cython_7_bitset_bitset_iterator_func, ((void *)__pyx_v_func));
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":205
+      /* "pybitset/backends/cython/_bitset.pyx":206
  *     cpdef inline bint for_each(self, object func):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)
  *         return ret
  */
       /*finally:*/ {
@@ -5720,25 +5740,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":207
+  /* "pybitset/backends/cython/_bitset.pyx":208
  *         with nogil:
  *             ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline print(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":203
+  /* "pybitset/backends/cython/_bitset.pyx":204
  *         return BitSetIter(self)
  * 
  *     cpdef inline bint for_each(self, object func):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -5767,15 +5787,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("for_each", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_for_each(__pyx_v_self, __pyx_v_func, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_for_each(__pyx_v_self, __pyx_v_func, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5784,54 +5804,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":209
+/* "pybitset/backends/cython/_bitset.pyx":210
  *         return ret
  * 
  *     cpdef inline print(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_print(self._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_65print(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_print(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("print", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":210
+  /* "pybitset/backends/cython/_bitset.pyx":211
  * 
  *     cpdef inline print(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_print(self._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":211
+        /* "pybitset/backends/cython/_bitset.pyx":212
  *     cpdef inline print(self):
  *         with nogil:
  *             bitset_print(self._bitset)             # <<<<<<<<<<<<<<
  * 
  * @cython.internal
  */
         bitset_print(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":210
+      /* "pybitset/backends/cython/_bitset.pyx":211
  * 
  *     cpdef inline print(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_print(self._bitset)
  * 
  */
       /*finally:*/ {
@@ -5842,15 +5862,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":209
+  /* "pybitset/backends/cython/_bitset.pyx":210
  *         return ret
  * 
  *     cpdef inline print(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_print(self._bitset)
  */
 
@@ -5880,15 +5900,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("print", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_print(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_print(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6012,15 +6032,15 @@
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":222
+/* "pybitset/backends/cython/_bitset.pyx":223
  *         size_t i
  * 
  *     def __cinit__(self, BitSet b):             # <<<<<<<<<<<<<<
  *         self.b = b
  *         self.i = 0
  */
 
@@ -6049,32 +6069,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 222, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 223, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_b = ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 222, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 223, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSetIter.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b", 0))) __PYX_ERR(0, 222, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b", 0))) __PYX_ERR(0, 223, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_10BitSetIter___cinit__(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter *)__pyx_v_self), __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -6083,51 +6103,51 @@
 }
 
 static int __pyx_pf_8pybitset_8backends_6cython_7_bitset_10BitSetIter___cinit__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":223
+  /* "pybitset/backends/cython/_bitset.pyx":224
  * 
  *     def __cinit__(self, BitSet b):
  *         self.b = b             # <<<<<<<<<<<<<<
  *         self.i = 0
  * 
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_b));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_b));
   __Pyx_GOTREF(__pyx_v_self->b);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->b));
   __pyx_v_self->b = __pyx_v_b;
 
-  /* "pybitset/backends/cython/_bitset.pyx":224
+  /* "pybitset/backends/cython/_bitset.pyx":225
  *     def __cinit__(self, BitSet b):
  *         self.b = b
  *         self.i = 0             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_v_self->i = 0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":222
+  /* "pybitset/backends/cython/_bitset.pyx":223
  *         size_t i
  * 
  *     def __cinit__(self, BitSet b):             # <<<<<<<<<<<<<<
  *         self.b = b
  *         self.i = 0
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":226
+/* "pybitset/backends/cython/_bitset.pyx":227
  *         self.i = 0
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -6145,42 +6165,42 @@
 }
 
 static PyObject *__pyx_pf_8pybitset_8backends_6cython_7_bitset_10BitSetIter_2__iter__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":227
+  /* "pybitset/backends/cython/_bitset.pyx":228
  * 
  *     def __iter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":226
+  /* "pybitset/backends/cython/_bitset.pyx":227
  *         self.i = 0
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":229
+/* "pybitset/backends/cython/_bitset.pyx":230
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):
  */
 
@@ -6205,77 +6225,77 @@
   size_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":231
+  /* "pybitset/backends/cython/_bitset.pyx":232
  *     def __next__(self):
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):             # <<<<<<<<<<<<<<
  *             tmp = self.i
  *             self.i += 1
  */
   __pyx_t_1 = (bitset_next_set_bit(__pyx_v_self->b->_bitset, (&__pyx_v_self->i)) != 0);
   if (likely(__pyx_t_1)) {
 
-    /* "pybitset/backends/cython/_bitset.pyx":232
+    /* "pybitset/backends/cython/_bitset.pyx":233
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):
  *             tmp = self.i             # <<<<<<<<<<<<<<
  *             self.i += 1
  *             return tmp
  */
     __pyx_t_2 = __pyx_v_self->i;
     __pyx_v_tmp = __pyx_t_2;
 
-    /* "pybitset/backends/cython/_bitset.pyx":233
+    /* "pybitset/backends/cython/_bitset.pyx":234
  *         if bitset_next_set_bit(self.b._bitset, &self.i):
  *             tmp = self.i
  *             self.i += 1             # <<<<<<<<<<<<<<
  *             return tmp
  *         else:
  */
     __pyx_v_self->i = (__pyx_v_self->i + 1);
 
-    /* "pybitset/backends/cython/_bitset.pyx":234
+    /* "pybitset/backends/cython/_bitset.pyx":235
  *             tmp = self.i
  *             self.i += 1
  *             return tmp             # <<<<<<<<<<<<<<
  *         else:
  *             raise StopIteration
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_tmp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_tmp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 235, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "pybitset/backends/cython/_bitset.pyx":231
+    /* "pybitset/backends/cython/_bitset.pyx":232
  *     def __next__(self):
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):             # <<<<<<<<<<<<<<
  *             tmp = self.i
  *             self.i += 1
  */
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":236
+  /* "pybitset/backends/cython/_bitset.pyx":237
  *             return tmp
  *         else:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  */
   /*else*/ {
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 236, __pyx_L1_error)
+    __PYX_ERR(0, 237, __pyx_L1_error)
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":229
+  /* "pybitset/backends/cython/_bitset.pyx":230
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):
  */
 
@@ -6737,15 +6757,15 @@
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 34, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 237, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -6880,22 +6900,22 @@
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet.tp_dictoffset && __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   if (__Pyx_SetVtable(__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet.tp_dict, __pyx_vtabptr_8pybitset_8backends_6cython_7_bitset_BitSet) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BitSet, (PyObject *)&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet = &__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet;
-  if (PyType_Ready(&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter.tp_dictoffset && __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
   __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSetIter = &__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
```

### Comparing `pybitset-0.0.1.dev2/pybitset/backends/cython/_bitset.pyx` & `pybitset-0.0.1rc1/pybitset/backends/cython/_bitset.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
                 self._bitset = bitset_create_with_capacity(size)
             if not self._bitset:
                 raise MemoryError
         else:
             self._bitset = NULL
 
     def __dealloc__(self):
-        bitset_free(self._bitset)
+        if self._bitset:
+            bitset_free(self._bitset)
         self._bitset = NULL
 
     @staticmethod
     cdef inline BitSet from_ptr(bitset_t * ptr):
         cdef BitSet self = BitSet(_init=False)
         self._bitset = ptr
         return self
```

### Comparing `pybitset-0.0.1.dev2/pybitset/backends/cython/bitset.pxd` & `pybitset-0.0.1rc1/pybitset/backends/cython/bitset.pxd`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/pybitset.egg-info/PKG-INFO` & `pybitset-0.0.1rc1/pybitset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybitset
-Version: 0.0.1.dev2
+Version: 0.0.1rc1
 Summary: python binding for cbitset
 Home-page: https://github.com/synodriver/pybitset
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: BSD
 Keywords: bitset
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pybitset-0.0.1.dev2/pybitset.egg-info/SOURCES.txt` & `pybitset-0.0.1rc1/pybitset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybitset-0.0.1.dev2/setup.py` & `pybitset-0.0.1rc1/setup.py`

 * *Files identical despite different names*

