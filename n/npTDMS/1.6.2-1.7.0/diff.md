# Comparing `tmp/npTDMS-1.6.2.tar.gz` & `tmp/npTDMS-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npTDMS-1.6.2.tar", last modified: Sun Mar 26 23:57:15 2023, max compression
+gzip compressed data, was "npTDMS-1.7.0.tar", last modified: Wed Jun 21 21:47:46 2023, max compression
```

## Comparing `npTDMS-1.6.2.tar` & `npTDMS-1.7.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.920917 npTDMS-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-26 23:57:15.000000 npTDMS-1.6.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-03-26 23:57:15.000000 npTDMS-1.6.2/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-26 23:57:15.000000 npTDMS-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-03-26 23:57:15.920917 npTDMS-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-26 23:57:15.000000 npTDMS-1.6.2/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-03-26 23:57:15.000000 npTDMS-1.6.2/coverage.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.908917 npTDMS-1.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/apireference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/reading.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/tdmsinfo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-26 23:57:15.000000 npTDMS-1.6.2/docs/writing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.912917 npTDMS-1.6.2/npTDMS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-03-26 23:57:15.000000 npTDMS-1.6.2/npTDMS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-26 23:57:15.000000 npTDMS-1.6.2/npTDMS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 23:57:15.000000 npTDMS-1.6.2/npTDMS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-26 23:57:15.000000 npTDMS-1.6.2/npTDMS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-26 23:57:15.000000 npTDMS-1.6.2/npTDMS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-26 23:57:15.000000 npTDMS-1.6.2/npTDMS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.916917 npTDMS-1.6.2/nptdms/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/base_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/channel_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/daqmx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.916917 npTDMS-1.6.2/nptdms/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/export/hdf_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/export/pandas_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    27419 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    35895 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/tdms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/tdms_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/tdmsinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.920917 npTDMS-1.6.2/nptdms/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.920917 npTDMS-1.6.2/nptdms/test/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23819 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/data/Digital_Input.tdms
--rw-r--r--   0 runner    (1001) docker     (123)    57171 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/data/big_endian.tdms
--rwxr-xr-x   0 runner    (1001) docker     (123)    34568 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/data/raw1.tdms
--rw-r--r--   0 runner    (1001) docker     (123)    32485 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    35779 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_daqmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_example_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    31229 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    42605 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_tdms_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_tdmsinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_thermocouples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.920917 npTDMS-1.6.2/nptdms/test/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/writer/test_acceptance_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/test/writer/test_tdms_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/thermocouples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-03-26 23:57:15.000000 npTDMS-1.6.2/nptdms/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-26 23:57:15.000000 npTDMS-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-26 23:57:15.920917 npTDMS-1.6.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-03-26 23:57:15.000000 npTDMS-1.6.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-26 23:57:15.000000 npTDMS-1.6.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:46.738258 npTDMS-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-21 21:47:45.000000 npTDMS-1.7.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-21 21:47:45.000000 npTDMS-1.7.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-21 21:47:45.000000 npTDMS-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-21 21:47:46.738258 npTDMS-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-21 21:47:45.000000 npTDMS-1.7.0/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-06-21 21:47:45.000000 npTDMS-1.7.0/coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:46.734257 npTDMS-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/apireference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/reading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/tdmsinfo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-21 21:47:45.000000 npTDMS-1.7.0/docs/writing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:46.734257 npTDMS-1.7.0/npTDMS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-21 21:47:46.000000 npTDMS-1.7.0/npTDMS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-21 21:47:46.000000 npTDMS-1.7.0/npTDMS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:47:46.000000 npTDMS-1.7.0/npTDMS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 21:47:46.000000 npTDMS-1.7.0/npTDMS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-21 21:47:46.000000 npTDMS-1.7.0/npTDMS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 21:47:46.000000 npTDMS-1.7.0/npTDMS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:46.734257 npTDMS-1.7.0/nptdms/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/base_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/channel_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/daqmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:46.738258 npTDMS-1.7.0/nptdms/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/export/hdf_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/export/pandas_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27419 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35895 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/tdms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/tdms_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/tdmsinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:46.738258 npTDMS-1.7.0/nptdms/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:46.738258 npTDMS-1.7.0/nptdms/test/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23819 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/data/Digital_Input.tdms
+-rw-r--r--   0 runner    (1001) docker     (123)    57171 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/data/big_endian.tdms
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34568 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/data/raw1.tdms
+-rw-r--r--   0 runner    (1001) docker     (123)    32485 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35779 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_daqmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_example_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31229 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42605 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_tdms_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_tdmsinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_thermocouples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:46.738258 npTDMS-1.7.0/nptdms/test/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/writer/test_tdms_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/test/writer/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/thermocouples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-21 21:47:45.000000 npTDMS-1.7.0/nptdms/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 21:47:45.000000 npTDMS-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-21 21:47:46.738258 npTDMS-1.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-21 21:47:45.000000 npTDMS-1.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 21:47:45.000000 npTDMS-1.7.0/tox.ini
```

### Comparing `npTDMS-1.6.2/COPYING` & `npTDMS-1.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/COPYING.LESSER` & `npTDMS-1.7.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/PKG-INFO` & `npTDMS-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npTDMS
-Version: 1.6.2
+Version: 1.7.0
 Summary: Cross-platform, NumPy based module for reading TDMS files produced by LabView
 Home-page: https://github.com/adamreeve/npTDMS
 Author: Adam Reeve
 Author-email: adreeve@gmail.com
 License: LGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `npTDMS-1.6.2/README.rst` & `npTDMS-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/docs/Makefile` & `npTDMS-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/docs/apireference.rst` & `npTDMS-1.7.0/docs/apireference.rst`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/docs/conf.py` & `npTDMS-1.7.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import sys, os
+import configparser
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('..'))
 
 # -- General configuration -----------------------------------------------------
@@ -46,21 +47,20 @@
 project = u'npTDMS'
 copyright = u'2012, Adam Reeve'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-v_globals = {}
-v_locals = {}
-exec(open('../nptdms/version.py').read(), v_globals, v_locals)
+setup_cfg = configparser.ConfigParser()
+setup_cfg.read('../setup.cfg')
 # The short X.Y version.
-version = '.'.join('%d' % d for d in v_locals['__version_info__'][:2])
+version = '.'.join(setup_cfg['metadata']['version'].split('.')[:2])
 # The full version, including alpha/beta/rc tags.
-release = v_locals['__version__']
+release = setup_cfg['metadata']['version']
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `npTDMS-1.6.2/docs/quickstart.rst` & `npTDMS-1.7.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/docs/reading.rst` & `npTDMS-1.7.0/docs/reading.rst`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/docs/tdmsinfo.rst` & `npTDMS-1.7.0/docs/tdmsinfo.rst`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/docs/writing.rst` & `npTDMS-1.7.0/docs/writing.rst`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/npTDMS.egg-info/PKG-INFO` & `npTDMS-1.7.0/npTDMS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npTDMS
-Version: 1.6.2
+Version: 1.7.0
 Summary: Cross-platform, NumPy based module for reading TDMS files produced by LabView
 Home-page: https://github.com/adamreeve/npTDMS
 Author: Adam Reeve
 Author-email: adreeve@gmail.com
 License: LGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `npTDMS-1.6.2/npTDMS.egg-info/SOURCES.txt` & `npTDMS-1.7.0/npTDMS.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -56,9 +56,9 @@
 nptdms/test/test_timestamps.py
 nptdms/test/test_types.py
 nptdms/test/util.py
 nptdms/test/data/Digital_Input.tdms
 nptdms/test/data/big_endian.tdms
 nptdms/test/data/raw1.tdms
 nptdms/test/writer/__init__.py
-nptdms/test/writer/test_acceptance_tests.py
-nptdms/test/writer/test_tdms_segment.py
+nptdms/test/writer/test_tdms_segment.py
+nptdms/test/writer/test_writer.py
```

### Comparing `npTDMS-1.6.2/nptdms/base_segment.py` & `npTDMS-1.7.0/nptdms/base_segment.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/channel_data.py` & `npTDMS-1.7.0/nptdms/channel_data.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/common.py` & `npTDMS-1.7.0/nptdms/common.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/daqmx.py` & `npTDMS-1.7.0/nptdms/daqmx.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/export/hdf_export.py` & `npTDMS-1.7.0/nptdms/export/hdf_export.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/export/pandas_export.py` & `npTDMS-1.7.0/nptdms/export/pandas_export.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/log.py` & `npTDMS-1.7.0/nptdms/log.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/reader.py` & `npTDMS-1.7.0/nptdms/reader.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/scaling.py` & `npTDMS-1.7.0/nptdms/scaling.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/tdms.py` & `npTDMS-1.7.0/nptdms/tdms.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/tdms_segment.py` & `npTDMS-1.7.0/nptdms/tdms_segment.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/tdmsinfo.py` & `npTDMS-1.7.0/nptdms/tdmsinfo.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/data/Digital_Input.tdms` & `npTDMS-1.7.0/nptdms/test/data/Digital_Input.tdms`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/data/big_endian.tdms` & `npTDMS-1.7.0/nptdms/test/data/big_endian.tdms`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/data/raw1.tdms` & `npTDMS-1.7.0/nptdms/test/data/raw1.tdms`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/scenarios.py` & `npTDMS-1.7.0/nptdms/test/scenarios.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_benchmarks.py` & `npTDMS-1.7.0/nptdms/test/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_daqmx.py` & `npTDMS-1.7.0/nptdms/test/test_daqmx.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_example_files.py` & `npTDMS-1.7.0/nptdms/test/test_example_files.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_hdf.py` & `npTDMS-1.7.0/nptdms/test/test_hdf.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_pandas.py` & `npTDMS-1.7.0/nptdms/test/test_pandas.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_scaling.py` & `npTDMS-1.7.0/nptdms/test/test_scaling.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_tdms_file.py` & `npTDMS-1.7.0/nptdms/test/test_tdms_file.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_tdmsinfo.py` & `npTDMS-1.7.0/nptdms/test/test_tdmsinfo.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_thermocouples.py` & `npTDMS-1.7.0/nptdms/test/test_thermocouples.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_timestamps.py` & `npTDMS-1.7.0/nptdms/test/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/test_types.py` & `npTDMS-1.7.0/nptdms/test/test_types.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/util.py` & `npTDMS-1.7.0/nptdms/test/util.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/test/writer/test_acceptance_tests.py` & `npTDMS-1.7.0/nptdms/test/writer/test_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -399,7 +399,93 @@
     output_file = BytesIO()
 
     with pytest.raises(ValueError) as exception:
         _ = TdmsWriter(output_file, version=4714)
     error_message = str(exception.value)
 
     assert "4712,4713" in error_message
+
+
+def test_root_object_added():
+    """ When not explicitly included, a root object should be added
+    """
+    group = GroupObject("group")
+    channel = ChannelObject("group", "a", np.linspace(0.0, 1.0, 10))
+
+    output_file = BytesIO()
+    with TdmsWriter(output_file) as tdms_writer:
+        tdms_writer.write_segment([group, channel])
+        tdms_writer.write_segment([group, channel])
+
+    output_file.seek(0)
+
+    tdms_file = TdmsFile(output_file)
+    first_segment_objects = tdms_file._reader._segments[0].ordered_objects
+    second_segment_objects = tdms_file._reader._segments[1].ordered_objects
+
+    assert first_segment_objects[0].path == "/"
+    assert not any(obj.path == "/" for obj in second_segment_objects)
+
+
+def test_group_object_added():
+    """ When not explicitly included, a group object should be added
+    """
+    root = RootObject()
+    channel = ChannelObject("group", "a", np.linspace(0.0, 1.0, 10))
+
+    output_file = BytesIO()
+    with TdmsWriter(output_file) as tdms_writer:
+        tdms_writer.write_segment([root, channel])
+        tdms_writer.write_segment([root, channel])
+
+    output_file.seek(0)
+
+    tdms_file = TdmsFile(output_file)
+    first_segment_objects = tdms_file._reader._segments[0].ordered_objects
+    second_segment_objects = tdms_file._reader._segments[1].ordered_objects
+
+    assert first_segment_objects[1].path == "/'group'"
+    assert not any(obj.path == "/'group'" for obj in second_segment_objects)
+
+
+def test_group_not_duplicated():
+    root = RootObject()
+    group = GroupObject("group")
+    channel = ChannelObject("group", "a", np.linspace(0.0, 1.0, 10))
+
+    output_file = BytesIO()
+    with TdmsWriter(output_file) as tdms_writer:
+        tdms_writer.write_segment([root, group, channel])
+        tdms_writer.write_segment([channel])
+
+    output_file.seek(0)
+
+    tdms_file = TdmsFile(output_file)
+    first_segment_objects = tdms_file._reader._segments[0].ordered_objects
+    second_segment_objects = tdms_file._reader._segments[1].ordered_objects
+
+    assert len(first_segment_objects) == 3
+    assert len(second_segment_objects) == 1
+
+
+def test_root_and_groups_ordered_first():
+    """
+    The root and group objects should always come first
+    """
+    root = RootObject()
+    group = GroupObject("group")
+    channel_0 = ChannelObject("group", "b", np.linspace(0.0, 1.0, 10))
+    channel_1 = ChannelObject("group", "a", np.linspace(0.0, 1.0, 10))
+
+    output_file = BytesIO()
+    with TdmsWriter(output_file) as tdms_writer:
+        tdms_writer.write_segment([channel_0, group, channel_1, root])
+
+    output_file.seek(0)
+
+    tdms_file = TdmsFile(output_file)
+    first_segment_objects = tdms_file._reader._segments[0].ordered_objects
+
+    assert first_segment_objects[0].path == "/"
+    assert first_segment_objects[1].path == "/'group'"
+    assert first_segment_objects[2].path == "/'group'/'b'"
+    assert first_segment_objects[3].path == "/'group'/'a'"
```

### Comparing `npTDMS-1.6.2/nptdms/test/writer/test_tdms_segment.py` & `npTDMS-1.7.0/nptdms/test/writer/test_tdms_segment.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/thermocouples.py` & `npTDMS-1.7.0/nptdms/thermocouples.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/timestamp.py` & `npTDMS-1.7.0/nptdms/timestamp.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/types.py` & `npTDMS-1.7.0/nptdms/types.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/utils.py` & `npTDMS-1.7.0/nptdms/utils.py`

 * *Files identical despite different names*

### Comparing `npTDMS-1.6.2/nptdms/writer.py` & `npTDMS-1.7.0/nptdms/writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,29 +60,31 @@
             This will be passed through to Python's ``open`` function with 'b' appended
             to ensure the file is opened in binary mode.
             For example, use 'w' (the default) to open a new file or 'a' to append to an existing TDMS file.
         :param version: The TDMS format version to write, which must be either 4712 (the default) or 4713.
             It's important that if you are appending segments to an
             existing TDMS file, this matches the existing file version (this can be queried with the
             :py:attr:`~nptdms.TdmsFile.tdms_version` property).
-        :param index_file: Whether or not to write a index file besides the data file. Index files
+        :param index_file: Whether to write an index file besides the data file. Index files
             can be used to accelerate reading speeds for faster channel extraction and data positions inside
-            the data files. If ``file```variable is a path ``index_file`` can be ``True`` to store a ``.tdms_index``
-            file at the same folder location or ``False`` to only write the data ``.tdms`` file. If ``file`` variable
-            is a readable object ``index_file`` can either be a readable object to write into or ``False`` to omit.
+            the data files. If ``file```variable is a path, ``index_file`` can be ``True`` to store a ``.tdms_index``
+            file at the same folder location or ``False`` to only write the data ``.tdms`` file. If ``file``
+            is a readable object, ``index_file`` can either be a readable object to write into or ``False`` to omit.
         """
         valid_versions = (4712, 4713)
         if version not in valid_versions:
             raise ValueError("version must be one of %s" % ",".join("%d" % v for v in valid_versions))
         self._file = None
         self._index_file = None
         self._file_path = None
         self._index_file_path = None
         self._file_mode = mode
         self._tdms_version = version
+        self._root_written = False
+        self._groups_written = set()
 
         if hasattr(file, "read"):
             # Is a file
             self._file = file
             if hasattr(index_file, "read"):
                 self._index_file = index_file
             elif isinstance(index_file, bool) and not index_file:
@@ -119,21 +121,45 @@
         self._index_file = None
 
     def write_segment(self, objects):
         """ Write a segment of data to a TDMS file
 
         :param objects: A list of TdmsObject instances to write
         """
+        path_object_pairs = [(ObjectPath.from_string(o.path), o) for o in objects]
+
+        # Make sure a root object is included if this is the first segment,
+        # and any groups used by channels have associated group objects
+        add_root = (not self._root_written) and (not any(p[0].is_root for p in path_object_pairs))
+        groups_included = set(p[0].group for p in path_object_pairs if p[0].is_group)
+        groups_required = set(p[0].group for p in path_object_pairs if p[0].is_channel)
+        groups_to_add = sorted(groups_required - groups_included - self._groups_written)
+
+        if add_root:
+            path_object_pairs.append((ObjectPath(), RootObject()))
+        if groups_to_add:
+            path_object_pairs.extend((ObjectPath(g), GroupObject(g)) for g in groups_to_add)
+
+        # Ensure objects are ordered with root first, then groups, in case any readers depend
+        # on parent objects being defined before their children.
+        # Channel ordering will be unchanged as sorts are stable.
+        path_object_pairs.sort(key=lambda p: _path_ordering_key(p[0]))
+
+        objects = [p[1] for p in path_object_pairs]
         segment = TdmsSegment(objects, version=self._tdms_version)
         segment.write(self._file)
 
         if self._index_file is not None:
             segment = TdmsSegment(objects, is_index_file=True, version=self._tdms_version)
             segment.write(self._index_file)
 
+        self._root_written = True
+        self._groups_written.update(groups_included)
+        self._groups_written.update(groups_to_add)
+
     def __enter__(self):
         self.open()
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.close()
 
@@ -446,7 +472,16 @@
         elif max_value >= 2**8 or min_value < -1 * 2**7:
             return np.dtype('int16')
         elif max_value >= 2**7 and min_value >= 0:
             return np.dtype('uint8')
         else:
             return np.dtype('int8')
     return None
+
+
+def _path_ordering_key(path):
+    if path.is_root:
+        return 0
+    if path.is_group:
+        return 1
+    if path.is_channel:
+        return 2
```

### Comparing `npTDMS-1.6.2/setup.cfg` & `npTDMS-1.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = npTDMS
-version = 1.6.2
+version = 1.7.0
 description = Cross-platform, NumPy based module for reading TDMS files produced by LabView
 author = Adam Reeve
 author_email = adreeve@gmail.com
 url = https://github.com/adamreeve/npTDMS
 long_description = file: README.rst
 license = LGPL
 classifiers =
```

