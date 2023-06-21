# Comparing `tmp/tiledbsoma-1.2.5.tar.gz` & `tmp/tiledbsoma-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.2.5.tar", last modified: Tue May 30 20:56:37 2023, max compression
+gzip compressed data, was "tiledbsoma-1.2.7.tar", last modified: Wed Jun 21 16:57:14 2023, max compression
```

## Comparing `tiledbsoma-1.2.5.tar` & `tiledbsoma-1.2.7.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-30 20:56:36.000000 tiledbsoma-1.2.5/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/cli/cli.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/
--rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10181 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (122)    14643 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15637 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_array.h
--rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (122)     9491 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_group.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (122)     7272 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/carrow.h
--rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/logger.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/logger.h
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/stats.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/stats.h
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/util.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/util.h
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/version.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/version.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.791899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_soma_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.791899 tiledbsoma-1.2.5/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/bld
--rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.791899 tiledbsoma-1.2.5/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     5370 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7213 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    33854 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (122)    11918 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7628 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    55615 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    11206 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/query_condition.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5107 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/cli/cli.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.619202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.619202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10181 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14643 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15637 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_array.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     9491 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_group.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.627203 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.627203 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7272 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/carrow.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/logger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/stats.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/util.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/version.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/version.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.627203 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_soma_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.627203 tiledbsoma-1.2.7/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/bld
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11110 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     5370 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7213 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33854 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11918 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7628 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56332 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11206 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/query_condition.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5107 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/version.py
```

### Comparing `tiledbsoma-1.2.5/PKG-INFO` & `tiledbsoma-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.5
+Version: 1.2.7
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
@@ -123,10 +123,11 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `tiledbsoma-1.2.5/README.md` & `tiledbsoma-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/cli/cli.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/cli/cli.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/.clang-format` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/span/span.hpp` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/logger_public.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/logger_public.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/managed_query.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/managed_query.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/managed_query.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_array.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_array.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_array.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_group.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_group.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_group.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/array_buffers.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/array_buffers.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/arrow_adapter.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/arrow_adapter.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/carrow.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/carrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/column_buffer.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/column_buffer.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/column_buffer.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/common.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/logger.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/logger.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/logger.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/logger.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/stats.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/stats.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/stats.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/stats.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/util.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/util.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/util.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/util.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/version.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/version.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/version.h` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/version.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_query_condition.py` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_simple.py` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_soma_array.py` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_soma_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_soma_array.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_soma_group.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/scripts/bld` & `tiledbsoma-1.2.7/dist_links/scripts/bld`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.2.7/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/scripts/show-versions.py` & `tiledbsoma-1.2.7/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.2.7/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/setup.py` & `tiledbsoma-1.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,14 +243,15 @@
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages("src"),
     # This next is necessary to avoid cibuildwheel thinking we want a python-only wheel:
     ext_modules=[
         Pybind11Extension(
             "tiledbsoma.pytiledbsoma",
@@ -278,16 +279,17 @@
         # with less-particular numpy version constraints, or if we decide we no
         # longer need to support the old pip solver (default on ubuntu 20.04).
         #
         # Also: numba doesn't support Python 3.11 until 0.57.0rc1.
         # It' not preferable to pin to an RC dependency, so we only do this
         # when we must, which is for 3.11.
         "numba==0.56.4; python_version<'3.11'",
-        "numba==0.57.0rc1; python_version=='3.11'",
-        "numpy>=1.18,<1.24",
+        "numba==0.57; python_version=='3.11'",
+        "numpy>=1.18,<1.24; python_version<'3.11'",
+        "numpy>=1.18,<1.25; python_version=='3.11'",
         "pandas",
         "pyarrow>=9.0.0",
         "scanpy>=1.9.2",
         "scipy",
         "somacore==1.0.3",
         "tiledb~=0.21.3",
         "typing-extensions",  # Note "-" even though `import typing_extensions`
```

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/__init__.py` & `tiledbsoma-1.2.7/src/tiledbsoma/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_arrow_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_collection.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_collection.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_common_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_dense_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_exception.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_exception.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_experiment.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_factory.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_factory.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_general_utilities.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_measurement.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_read_iters.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_sparse_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_tdb_handles.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_tiledb_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_tiledb_object.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_types.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/_util.py` & `tiledbsoma-1.2.7/src/tiledbsoma/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/eta.py` & `tiledbsoma-1.2.7/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.2.7/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.2.7/src/tiledbsoma/io/conversions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.2.7/src/tiledbsoma/io/ingest.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,14 +329,27 @@
                     anndata.X,
                     platform_config,
                     ingest_mode,
                     context,
                 ) as data:
                     _maybe_set(x, "data", data, use_relative_uri=use_relative_uri)
 
+                for layer_name, layer in anndata.layers.items():
+                    with create_from_matrix(
+                        X_kind,
+                        _util.uri_joinpath(measurement_X_uri, layer_name),
+                        layer,
+                        platform_config,
+                        ingest_mode,
+                        context,
+                    ) as layer_data:
+                        _maybe_set(
+                            x, layer_name, layer_data, use_relative_uri=use_relative_uri
+                        )
+
                 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
                 # MS/meas/OBSM,VARM,OBSP,VARP
                 if len(anndata.obsm.keys()) > 0:  # do not create an empty collection
                     obsm_uri = _util.uri_joinpath(measurement_uri, "obsm")
                     with _create_or_open_coll(
                         Collection,
                         obsm_uri,
@@ -1284,14 +1297,20 @@
     value: NPNDArray,
     platform_config: Optional[PlatformConfig],
     context: Optional[SOMATileDBContext],
     *,
     use_relative_uri: Optional[bool],
 ) -> None:
     arr_uri = _util.uri_joinpath(coll.uri, key)
+
+    if any(e <= 0 for e in value.shape):
+        msg = f"Skipped {arr_uri} (uns ndarray): zero in shape {value.shape}"
+        logging.log_io(msg, msg)
+        return
+
     try:
         pa_dtype = pa.from_numpy_dtype(value.dtype)
     except pa.ArrowNotImplementedError:
         msg = (
             f"Skipped {arr_uri} (uns ndarray):"
             f" unsupported dtype {value.dtype!r} ({value.dtype})"
         )
```

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/logging.py` & `tiledbsoma-1.2.7/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.2.7/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/options/_tiledb_create_options.py` & `tiledbsoma-1.2.7/src/tiledbsoma/options/_tiledb_create_options.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.2.7/src/tiledbsoma/pytiledbsoma.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.2.7/src/tiledbsoma/query_condition.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.2.7/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.5
+Version: 1.2.7
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
@@ -123,10 +123,11 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `tiledbsoma-1.2.5/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.2.7/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.5/version.py` & `tiledbsoma-1.2.7/version.py`

 * *Files identical despite different names*

