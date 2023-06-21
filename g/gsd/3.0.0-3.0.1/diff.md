# Comparing `tmp/gsd-3.0.0.tar.gz` & `tmp/gsd-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsd-3.0.0.tar", last modified: Fri Jun 16 16:02:16 2023, max compression
+gzip compressed data, was "gsd-3.0.1.tar", last modified: Wed Jun 21 01:57:43 2023, max compression
```

## Comparing `gsd-3.0.0.tar` & `gsd-3.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:02:16.929646 gsd-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-16 16:02:02.000000 gsd-3.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-16 16:02:02.000000 gsd-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 16:02:02.000000 gsd-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-16 16:02:16.929646 gsd-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-16 16:02:02.000000 gsd-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:02:16.925646 gsd-3.0.0/gsd/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   722151 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd/fl.c
--rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/fl.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    73766 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/gsd.c
--rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/gsd.h
--rw-r--r--   0 runner    (1001) docker     (123)    45314 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/libgsd.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/pygsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/pytest_plugin_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:02:16.929646 gsd-3.0.0/gsd/test/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/test_fl.py
--rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/test_gsd_v1.gsd
--rw-r--r--   0 runner    (1001) docker     (123)    34233 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/test_hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/test/test_largefile.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-16 16:02:02.000000 gsd-3.0.0/gsd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:02:16.929646 gsd-3.0.0/gsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 16:02:16.000000 gsd-3.0.0/gsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-16 16:02:02.000000 gsd-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-16 16:02:16.929646 gsd-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 16:02:02.000000 gsd-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:57:43.773106 gsd-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-21 01:57:25.000000 gsd-3.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-21 01:57:25.000000 gsd-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-21 01:57:25.000000 gsd-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-21 01:57:43.773106 gsd-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-21 01:57:25.000000 gsd-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:57:43.769106 gsd-3.0.1/gsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   722151 2023-06-21 01:57:42.000000 gsd-3.0.1/gsd/fl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/fl.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    73766 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/gsd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/gsd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45314 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/libgsd.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/pygsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/pytest_plugin_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:57:43.773106 gsd-3.0.1/gsd/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/test/test_fl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/test/test_gsd_v1.gsd
+-rw-r--r--   0 runner    (1001) docker     (123)    34233 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/test/test_hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/test/test_largefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-21 01:57:25.000000 gsd-3.0.1/gsd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:57:43.769106 gsd-3.0.1/gsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-21 01:57:43.000000 gsd-3.0.1/gsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-21 01:57:43.000000 gsd-3.0.1/gsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:57:43.000000 gsd-3.0.1/gsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 01:57:43.000000 gsd-3.0.1/gsd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 01:57:43.000000 gsd-3.0.1/gsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-21 01:57:43.000000 gsd-3.0.1/gsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-21 01:57:25.000000 gsd-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-21 01:57:43.773106 gsd-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-21 01:57:25.000000 gsd-3.0.1/setup.py
```

### Comparing `gsd-3.0.0/CHANGELOG.rst` & `gsd-3.0.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 
 `GSD <https://github.com/glotzerlab/gsd>`_ releases follow `semantic versioning
 <https://semver.org/>`_.
 
 3.x
 ---
 
+3.0.1 (2023-06-20)
+^^^^^^^^^^^^^^^^^^
+
+*Fixed:*
+
+* Prevent ``ValueError: signal only works in main thread of the main interpreter`` when importing
+  gsd in a non-main thread.
+
 3.0.0 (2023-06-16)
 ^^^^^^^^^^^^^^^^^^
 
 *Added:*
 
 * ``gsd.version.version`` - version string identifier. PEP8 compliant name replaces ``__version__``.
 * ``GSDFile.flush`` - flush write buffers (C API ``gsd_flush``)
```

### Comparing `gsd-3.0.0/LICENSE` & `gsd-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/PKG-INFO` & `gsd-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 3.0.0
+Version: 3.0.1
 Summary: General simulation data file format.
 Author-email: "Joshua A. Anderson" <joaander@umich.edu>
 License: BSD-2-Clause
 Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.0.0/gsd-3.0.0.tar.gz
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.0.1/gsd-3.0.1.tar.gz
 Project-URL: Source, https://github.com/glotzerlab/gsd
 Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
```

### Comparing `gsd-3.0.0/README.md` & `gsd-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/__main__.py` & `gsd-3.0.1/gsd/__main__.py`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/fl.c` & `gsd-3.0.1/gsd/fl.c`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "gsd/gsd.h"
         ],
         "include_dirs": [
             "./gsd",
-            "/tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "gsd.fl",
         "sources": [
             "gsd/fl.pyx",
             "gsd/gsd.c"
         ]
     },
@@ -1069,195 +1069,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1285,42 +1285,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_3gsd_2fl_GSDFile;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -11071,15 +11071,15 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_WriteUnraisable("gsd.fl.GSDFile.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -11088,29 +11088,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -11121,15 +11121,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -11138,29 +11138,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -11171,15 +11171,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -11188,29 +11188,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -11221,15 +11221,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11238,29 +11238,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11271,15 +11271,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11288,29 +11288,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11321,212 +11321,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11542,15 +11542,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -11558,53 +11558,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -11612,30 +11612,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11650,15 +11650,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11674,15 +11674,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11690,53 +11690,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -11744,30 +11744,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11782,15 +11782,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11806,15 +11806,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11822,53 +11822,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -11876,30 +11876,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11914,176 +11914,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -12494,26 +12494,26 @@
  * 
  *         logger.info('truncating file: ' + self.name)
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_File_is_not_open); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 445, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -12979,15 +12979,15 @@
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../../../tmp/build-env-r1dzrzc_/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-cnvxjxzd/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `gsd-3.0.0/gsd/fl.pyx` & `gsd-3.0.1/gsd/fl.pyx`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/gsd.c` & `gsd-3.0.1/gsd/gsd.c`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/gsd.h` & `gsd-3.0.1/gsd/gsd.h`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/hoomd.py` & `gsd-3.0.1/gsd/hoomd.py`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/libgsd.pxd` & `gsd-3.0.1/gsd/libgsd.pxd`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/pygsd.py` & `gsd-3.0.1/gsd/pygsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from __future__ import division
 import logging
 import numpy
 import struct
 from collections import namedtuple
 import sys
 
-version = "3.0.0"
+version = "3.0.1"
 
 logger = logging.getLogger('gsd.pygsd')
 
 gsd_header = namedtuple(
     'gsd_header',
     'magic index_location index_allocated_entries '
     'namelist_location namelist_allocated_entries '
```

### Comparing `gsd-3.0.0/gsd/pytest_plugin_validate.py` & `gsd-3.0.1/gsd/pytest_plugin_validate.py`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/test/conftest.py` & `gsd-3.0.1/gsd/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/test/test_fl.py` & `gsd-3.0.1/gsd/test/test_fl.py`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/test/test_gsd_v1.gsd` & `gsd-3.0.1/gsd/test/test_gsd_v1.gsd`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/test/test_hoomd.py` & `gsd-3.0.1/gsd/test/test_hoomd.py`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd/test/test_largefile.py` & `gsd-3.0.1/gsd/test/test_largefile.py`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/gsd.egg-info/PKG-INFO` & `gsd-3.0.1/gsd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 3.0.0
+Version: 3.0.1
 Summary: General simulation data file format.
 Author-email: "Joshua A. Anderson" <joaander@umich.edu>
 License: BSD-2-Clause
 Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.0.0/gsd-3.0.0.tar.gz
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.0.1/gsd-3.0.1.tar.gz
 Project-URL: Source, https://github.com/glotzerlab/gsd
 Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
```

### Comparing `gsd-3.0.0/gsd.egg-info/SOURCES.txt` & `gsd-3.0.1/gsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/pyproject.toml` & `gsd-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 requires-python = ">=3.6"
 name = "gsd"
-version = "3.0.0"
+version = "3.0.1"
 description = "General simulation data file format."
 readme = "README.md"
 license = {text = "BSD-2-Clause"}
 authors = [
     {name = "Joshua A. Anderson", email = "joaander@umich.edu"},
 ]
 classifiers=[
@@ -21,15 +21,15 @@
 
 [project.scripts]
 gsd = "gsd.__main__:main"
 
 [project.urls]
 Homepage = "https://gsd.readthedocs.io"
 Documentation = "https://gsd.readthedocs.io"
-Download = "https://github.com/glotzerlab/gsd/releases/download/v3.0.0/gsd-3.0.0.tar.gz"
+Download = "https://github.com/glotzerlab/gsd/releases/download/v3.0.1/gsd-3.0.1.tar.gz"
 Source = "https://github.com/glotzerlab/gsd"
 Issues = "https://github.com/glotzerlab/gsd/issues"
 
 [tool.setuptools]
 packages = ["gsd", "gsd.test"]
 
 [build-system]
```

### Comparing `gsd-3.0.0/setup.cfg` & `gsd-3.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gsd-3.0.0/setup.py` & `gsd-3.0.1/setup.py`

 * *Files identical despite different names*

