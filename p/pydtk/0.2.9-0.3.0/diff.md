# Comparing `tmp/pydtk-0.2.9.tar.gz` & `tmp/pydtk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydtk-0.2.9.tar", max compression
+gzip compressed data, was "pydtk-0.3.0.tar", max compression
```

## Comparing `pydtk-0.2.9.tar` & `pydtk-0.3.0.tar`

### file list

```diff
@@ -1,120 +1,138 @@
--rw-r--r--   0        0        0    11340 2023-02-09 04:26:45.614931 pydtk-0.2.9/LICENSE
--rw-r--r--   0        0        0     2574 2023-02-09 04:26:45.614931 pydtk-0.2.9/README.md
--rw-r--r--   0        0        0      103 2023-02-09 04:27:01.803170 pydtk-0.2.9/pydtk/__init__.py
--rw-r--r--   0        0        0       44 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/__init__.py
--rwxr-xr-x   0        0        0     2184 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/cli.py
--rwxr-xr-x   0        0        0     3679 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/make_meta.py
--rw-r--r--   0        0        0     2631 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/oas.py
--rw-r--r--   0        0        0       28 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/__init__.py
--rw-r--r--   0        0        0    14844 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/db.py
--rw-r--r--   0        0        0      585 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/io.py
--rw-r--r--   0        0        0     4310 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/model.py
--rw-r--r--   0        0        0     1501 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/status.py
--rw-r--r--   0        0        0       44 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/__init__.py
--rwxr-xr-x   0        0        0     1578 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/concat_df.py
--rw-r--r--   0        0        0       44 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/dbdb/__init__.py
--rwxr-xr-x   0        0        0     5177 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/dbdb/file_info.py
--rwxr-xr-x   0        0        0     6453 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/df_list.py
--rwxr-xr-x   0        0        0     1696 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/df_path.py
--rwxr-xr-x   0        0        0     3473 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/meta_db.py
--rwxr-xr-x   0        0        0     6572 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/statistic_db.py
--rw-r--r--   0        0        0      697 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/conf/v1.yaml
--rw-r--r--   0        0        0     1477 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/conf/v2.yaml
--rw-r--r--   0        0        0     2553 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/conf/v3.yaml
--rw-r--r--   0        0        0     2185 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/conf/v4.yaml
--rw-r--r--   0        0        0     1093 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/__init__.py
--rw-r--r--   0        0        0      305 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/exceptions.py
--rw-r--r--   0        0        0     4114 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/__init__.py
--rw-r--r--   0        0        0      504 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation.py
--rw-r--r--   0        0        0     1123 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_pixel.py
--rw-r--r--   0        0        0     1387 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_rectangular_area.py
--rw-r--r--   0        0        0      903 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_point.py
--rw-r--r--   0        0        0      512 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/file.py
--rw-r--r--   0        0        0      399 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/record.py
--rw-r--r--   0        0        0        0 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/__init__.py
--rw-r--r--   0        0        0      540 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation.py
--rw-r--r--   0        0        0     1123 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_pixel.py
--rw-r--r--   0        0        0     1387 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_rectangular_area.py
--rw-r--r--   0        0        0      903 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_point.py
--rw-r--r--   0        0        0      891 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/file.py
--rw-r--r--   0        0        0      780 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/record.py
--rw-r--r--   0        0        0      193 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v1/__init__.py
--rw-r--r--   0        0        0     6508 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v1/handlers/__init__.py
--rw-r--r--   0        0        0     4913 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v1/handlers/meta.py
--rw-r--r--   0        0        0      360 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/__init__.py
--rw-r--r--   0        0        0    18716 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/handlers/__init__.py
--rw-r--r--   0        0        0     4519 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/handlers/meta.py
--rw-r--r--   0        0        0     1494 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/search_engines/__init__.py
--rw-r--r--   0        0        0     1813 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/search_engines/time_series.py
--rw-r--r--   0        0        0      562 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/__init__.py
--rw-r--r--   0        0        0    22454 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/handlers/__init__.py
--rw-r--r--   0        0        0    10185 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/handlers/meta.py
--rw-r--r--   0        0        0     4960 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/handlers/statistics.py
--rw-r--r--   0        0        0    12075 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/handlers/time_series.py
--rw-r--r--   0        0        0     4376 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/search_engines/__init__.py
--rw-r--r--   0        0        0     2409 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/search_engines/time_series.py
--rw-r--r--   0        0        0      288 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/__init__.py
--rw-r--r--   0        0        0      271 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/deps/__init__.py
--rw-r--r--   0        0        0       66 2023-02-09 04:26:46.118938 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/.git
--rw-r--r--   0        0        0       61 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/.gitignore
--rw-r--r--   0        0        0     1496 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/LICENSE
--rw-r--r--   0        0        0     7682 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/README.md
--rw-r--r--   0        0        0     5531 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/aggregation_tests.py
--rw-r--r--   0        0        0     7885 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/find_tests.py
--rw-r--r--   0        0        0     3066 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/__init__.py
--rw-r--r--   0        0        0     4848 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/aggregation.py
--rw-r--r--   0        0        0    14159 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/matching.py
--rw-r--r--   0        0        0      929 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/setup.py
--rw-r--r--   0        0        0       64 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/tox.ini
--rw-r--r--   0        0        0       66 2023-02-09 04:26:46.522944 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/.git
--rw-r--r--   0        0        0       61 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/.gitignore
--rw-r--r--   0        0        0     1496 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/LICENSE
--rw-r--r--   0        0        0     7682 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/README.md
--rw-r--r--   0        0        0     5531 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/aggregation_tests.py
--rw-r--r--   0        0        0     8389 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/find_tests.py
--rw-r--r--   0        0        0     3066 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/__init__.py
--rw-r--r--   0        0        0     4848 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/aggregation.py
--rw-r--r--   0        0        0    15543 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/matching.py
--rw-r--r--   0        0        0     1116 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/setup.py
--rw-r--r--   0        0        0      112 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/tox.ini
--rw-r--r--   0        0        0      954 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/__init__.py
--rw-r--r--   0        0        0     6354 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/mongodb.py
--rw-r--r--   0        0        0     5543 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/montydb.py
--rw-r--r--   0        0        0     2854 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/tinydb.py
--rw-r--r--   0        0        0     5716 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/tinymongo.py
--rw-r--r--   0        0        0    26623 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/db/v4/handlers/__init__.py
--rw-r--r--   0        0        0     3169 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/db/v4/handlers/annotation.py
--rw-r--r--   0        0        0    16709 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/db/v4/handlers/meta.py
--rwxr-xr-x   0        0        0     1456 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/frontend.py
--rw-r--r--   0        0        0      256 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/io/__init__.py
--rw-r--r--   0        0        0      187 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/io/errors.py
--rw-r--r--   0        0        0     4732 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/io/reader.py
--rw-r--r--   0        0        0     2459 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/io/writer.py
--rw-r--r--   0        0        0    18983 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/__init__.py
--rw-r--r--   0        0        0       67 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/autoware/__init__.py
--rw-r--r--   0        0        0     2402 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/autoware/can_packet.py
--rw-r--r--   0        0        0     6971 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/csv.py
--rw-r--r--   0        0        0     1991 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/image.py
--rw-r--r--   0        0        0     2308 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/json_model.py
--rw-r--r--   0        0        0    11798 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/movie.py
--rw-r--r--   0        0        0       58 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/pointcloud/__init__.py
--rw-r--r--   0        0        0     3413 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/pointcloud/pcd.py
--rw-r--r--   0        0        0    11181 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/rosbag.py
--rw-r--r--   0        0        0    14704 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/rosbag2.py
--rw-r--r--   0        0        0       65 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/zstd/__init__.py
--rw-r--r--   0        0        0     4374 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/zstd/rosbag.py
--rw-r--r--   0        0        0      131 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/preprocesses/__init__.py
--rwxr-xr-x   0        0        0     2527 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/preprocesses/downsampling.py
--rwxr-xr-x   0        0        0      929 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/preprocesses/passthrough.py
--rwxr-xr-x   0        0        0      352 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/preprocesses/preprocess.py
--rw-r--r--   0        0        0     3648 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/statistics/__init__.py
--rwxr-xr-x   0        0        0     8688 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/statistics/calculator.py
--rw-r--r--   0        0        0       44 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/utils/__init__.py
--rw-r--r--   0        0        0    18150 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/utils/can_decoder.py
--rwxr-xr-x   0        0        0     2728 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/utils/fileutils.py
--rwxr-xr-x   0        0        0     7478 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/utils/utils.py
--rwxr-xr-x   0        0        0     2591 2023-02-09 04:27:01.799170 pydtk-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     5489 2023-02-09 04:27:03.137252 pydtk-0.2.9/setup.py
--rw-r--r--   0        0        0     4661 2023-02-09 04:27:03.137844 pydtk-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-06-21 07:48:07.198635 pydtk-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2570 2023-06-21 07:48:07.198635 pydtk-0.3.0/README.md
+-rw-r--r--   0        0        0      103 2023-06-21 07:48:22.250693 pydtk-0.3.0/pydtk/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/__init__.py
+-rwxr-xr-x   0        0        0     2184 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/cli.py
+-rwxr-xr-x   0        0        0     3649 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/make_meta.py
+-rw-r--r--   0        0        0     2595 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/oas.py
+-rw-r--r--   0        0        0       28 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/sub_commands/__init__.py
+-rw-r--r--   0        0        0    14756 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/sub_commands/db.py
+-rw-r--r--   0        0        0      563 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/sub_commands/io.py
+-rw-r--r--   0        0        0     4272 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/sub_commands/model.py
+-rw-r--r--   0        0        0     1501 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/bin/sub_commands/status.py
+-rw-r--r--   0        0        0       44 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/builder/__init__.py
+-rwxr-xr-x   0        0        0     1578 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/builder/concat_df.py
+-rw-r--r--   0        0        0       44 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/builder/dbdb/__init__.py
+-rwxr-xr-x   0        0        0     5103 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/builder/dbdb/file_info.py
+-rwxr-xr-x   0        0        0     6439 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/builder/df_list.py
+-rwxr-xr-x   0        0        0     1696 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/builder/df_path.py
+-rwxr-xr-x   0        0        0     3473 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/builder/meta_db.py
+-rwxr-xr-x   0        0        0     6558 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/builder/statistic_db.py
+-rw-r--r--   0        0        0      697 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/conf/v1.yaml
+-rw-r--r--   0        0        0     1477 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/conf/v2.yaml
+-rw-r--r--   0        0        0     2553 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/conf/v3.yaml
+-rw-r--r--   0        0        0     2424 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/conf/v4.yaml
+-rw-r--r--   0        0        0     1093 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/exceptions.py
+-rw-r--r--   0        0        0     4028 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha1/__init__.py
+-rw-r--r--   0        0        0      504 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation.py
+-rw-r--r--   0        0        0     1019 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_pixel.py
+-rw-r--r--   0        0        0     1283 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_rectangular_area.py
+-rw-r--r--   0        0        0      813 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_point.py
+-rw-r--r--   0        0        0      512 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha1/file.py
+-rw-r--r--   0        0        0      399 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha1/record.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/__init__.py
+-rw-r--r--   0        0        0      541 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation.py
+-rw-r--r--   0        0        0     1019 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_pixel.py
+-rw-r--r--   0        0        0     1283 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_rectangular_area.py
+-rw-r--r--   0        0        0      813 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_point.py
+-rw-r--r--   0        0        0      891 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/file.py
+-rw-r--r--   0        0        0      780 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/record.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/__init__.py
+-rw-r--r--   0        0        0      541 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/annotation.py
+-rw-r--r--   0        0        0     1019 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/annotation_commented_image_pixel.py
+-rw-r--r--   0        0        0     1285 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/annotation_commented_image_rectangular_area.py
+-rw-r--r--   0        0        0      813 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/annotation_commented_point.py
+-rw-r--r--   0        0        0      891 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/file.py
+-rw-r--r--   0        0        0      780 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/record.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha4/__init__.py
+-rw-r--r--   0        0        0      574 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha4/annotation.py
+-rw-r--r--   0        0        0     1019 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha4/annotation_commented_image_pixel.py
+-rw-r--r--   0        0        0     1285 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha4/annotation_commented_image_rectangular_area.py
+-rw-r--r--   0        0        0      813 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha4/annotation_commented_point.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha5/__init__.py
+-rw-r--r--   0        0        0      574 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha5/annotation.py
+-rw-r--r--   0        0        0     1023 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha5/annotation_commented_image_pixel.py
+-rw-r--r--   0        0        0     1248 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha5/annotation_commented_image_rectangular_area.py
+-rw-r--r--   0        0        0      813 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha5/annotation_commented_point.py
+-rw-r--r--   0        0        0      820 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha5/arbitrary_annotation.py
+-rw-r--r--   0        0        0      193 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v1/__init__.py
+-rw-r--r--   0        0        0     6462 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v1/handlers/__init__.py
+-rw-r--r--   0        0        0     4875 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v1/handlers/meta.py
+-rw-r--r--   0        0        0      360 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v2/__init__.py
+-rw-r--r--   0        0        0    18286 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v2/handlers/__init__.py
+-rw-r--r--   0        0        0     4481 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v2/handlers/meta.py
+-rw-r--r--   0        0        0     1494 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v2/search_engines/__init__.py
+-rw-r--r--   0        0        0     1813 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v2/search_engines/time_series.py
+-rw-r--r--   0        0        0      562 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v3/__init__.py
+-rw-r--r--   0        0        0    21654 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v3/handlers/__init__.py
+-rw-r--r--   0        0        0     9873 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v3/handlers/meta.py
+-rw-r--r--   0        0        0     4772 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v3/handlers/statistics.py
+-rw-r--r--   0        0        0    11861 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v3/handlers/time_series.py
+-rw-r--r--   0        0        0     4376 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v3/search_engines/__init__.py
+-rw-r--r--   0        0        0     2383 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v3/search_engines/time_series.py
+-rw-r--r--   0        0        0      288 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v4/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v4/deps/__init__.py
+-rw-r--r--   0        0        0       66 2023-06-21 07:48:07.694637 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/.git
+-rw-r--r--   0        0        0       61 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/.gitignore
+-rw-r--r--   0        0        0     1496 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/LICENSE
+-rw-r--r--   0        0        0     7682 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/README.md
+-rw-r--r--   0        0        0     5531 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/aggregation_tests.py
+-rw-r--r--   0        0        0     7885 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/find_tests.py
+-rw-r--r--   0        0        0     3066 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/pql/__init__.py
+-rw-r--r--   0        0        0     4848 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/pql/aggregation.py
+-rw-r--r--   0        0        0    14159 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/pql/matching.py
+-rw-r--r--   0        0        0      929 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/setup.py
+-rw-r--r--   0        0        0       64 2023-06-21 07:48:09.038640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/tox.ini
+-rw-r--r--   0        0        0       66 2023-06-21 07:48:08.110638 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/.git
+-rw-r--r--   0        0        0       61 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/.gitignore
+-rw-r--r--   0        0        0     1496 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/LICENSE
+-rw-r--r--   0        0        0     7682 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/README.md
+-rw-r--r--   0        0        0     5531 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/aggregation_tests.py
+-rw-r--r--   0        0        0     8389 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/find_tests.py
+-rw-r--r--   0        0        0     3066 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/pql/__init__.py
+-rw-r--r--   0        0        0     4848 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/pql/aggregation.py
+-rw-r--r--   0        0        0    15543 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/pql/matching.py
+-rw-r--r--   0        0        0     1116 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/setup.py
+-rw-r--r--   0        0        0      112 2023-06-21 07:48:09.046640 pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/tox.ini
+-rw-r--r--   0        0        0      924 2023-06-21 07:48:07.202635 pydtk-0.3.0/pydtk/db/v4/engines/__init__.py
+-rw-r--r--   0        0        0     6284 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/db/v4/engines/mongodb.py
+-rw-r--r--   0        0        0     5531 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/db/v4/engines/montydb.py
+-rw-r--r--   0        0        0     2854 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/db/v4/engines/tinydb.py
+-rw-r--r--   0        0        0     5688 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/db/v4/engines/tinymongo.py
+-rw-r--r--   0        0        0    26376 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/db/v4/handlers/__init__.py
+-rw-r--r--   0        0        0     3048 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/db/v4/handlers/annotation.py
+-rw-r--r--   0        0        0    16169 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/db/v4/handlers/meta.py
+-rwxr-xr-x   0        0        0     1456 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/frontend.py
+-rw-r--r--   0        0        0      256 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/io/__init__.py
+-rw-r--r--   0        0        0      187 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/io/errors.py
+-rw-r--r--   0        0        0     4608 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/io/reader.py
+-rw-r--r--   0        0        0     2459 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/io/writer.py
+-rw-r--r--   0        0        0    18475 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/autoware/__init__.py
+-rw-r--r--   0        0        0     2336 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/autoware/can_packet.py
+-rw-r--r--   0        0        0     6941 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/csv.py
+-rw-r--r--   0        0        0     1969 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/image.py
+-rw-r--r--   0        0        0     2286 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/json_model.py
+-rw-r--r--   0        0        0    11670 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/movie.py
+-rw-r--r--   0        0        0       58 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/pointcloud/__init__.py
+-rw-r--r--   0        0        0     3413 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/pointcloud/pcd.py
+-rw-r--r--   0        0        0    11035 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/rosbag.py
+-rw-r--r--   0        0        0    14847 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/rosbag2.py
+-rw-r--r--   0        0        0       65 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/zstd/__init__.py
+-rw-r--r--   0        0        0     4344 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/models/zstd/rosbag.py
+-rw-r--r--   0        0        0      131 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/preprocesses/__init__.py
+-rwxr-xr-x   0        0        0     2527 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/preprocesses/downsampling.py
+-rwxr-xr-x   0        0        0      929 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/preprocesses/passthrough.py
+-rwxr-xr-x   0        0        0      352 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/preprocesses/preprocess.py
+-rw-r--r--   0        0        0     3626 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/statistics/__init__.py
+-rwxr-xr-x   0        0        0     8472 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/statistics/calculator.py
+-rw-r--r--   0        0        0       44 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/utils/__init__.py
+-rw-r--r--   0        0        0    17583 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/utils/can_decoder.py
+-rwxr-xr-x   0        0        0     2728 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/utils/fileutils.py
+-rw-r--r--   0        0        0      413 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/utils/imports.py
+-rwxr-xr-x   0        0        0     7443 2023-06-21 07:48:07.206635 pydtk-0.3.0/pydtk/utils/utils.py
+-rwxr-xr-x   0        0        0     2765 2023-06-21 07:48:22.246693 pydtk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 pydtk-0.3.0/PKG-INFO
```

### Comparing `pydtk-0.2.9/LICENSE` & `pydtk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/README.md` & `pydtk-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## Installation
 You can install the toolkit with:
 ```bash
 $ pip3 install pydtk
 
 ```
 
-If you want to install the toolkit with extra feature (e.g. support for PointCloud and ROS), 
+If you want to install the toolkit with extra feature (e.g. support for PointCloud and ROS),
 you can install it with extra dependencies as follows:
 ```bash
 $ pip3 install pydtk[pointcloud,ros]
 
 ```
 
 Some PyDTK models require additional packages.  
@@ -75,25 +75,25 @@
 
 
 ## Documentation
 For more information about this toolkit, please refer the [document](https://dataware-tools.github.io/pydtk/).
 
 
 ## Setup for contribution
-To improve this toolkit, firstly clone this repository and then 
-run the following command to prepare the environment. 
+To improve this toolkit, firstly clone this repository and then
+run the following command to prepare the environment.
 
 ```bash
 $ git clone git@github.com:dataware-tools/pydtk.git --recurse-submodules
 $ poetry install
 
 ```
 
 Make sure that [poetry](https://python-poetry.org/) is installed before executing the command.
 
-If you want to install the toolkit with extra feature (e.g. support for ROS), 
+If you want to install the toolkit with extra feature (e.g. support for ROS),
 please specify it with `-E` option.  
 Example (installation with `pointcloud` and `ros` extras):
 ```bash
 $ poetry install -E pointcloud -E ros
 
 ```
```

### Comparing `pydtk-0.2.9/pydtk/bin/cli.py` & `pydtk-0.3.0/pydtk/bin/cli.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/bin/make_meta.py` & `pydtk-0.3.0/pydtk/bin/make_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,17 +121,15 @@
     else:
         if args.file is None:
             raise ValueError("following arguments are required: --file")
         meta = make_meta(args.file, template)
         if args.out_dir is None:
             meta_json = None
         else:
-            meta_json = os.path.join(
-                args.out_dir, os.path.basename(args.file) + ".json"
-            )
+            meta_json = os.path.join(args.out_dir, os.path.basename(args.file) + ".json")
 
     with smart_open(meta_json, "wt") as f:
         json.dump(meta, f, indent=4)
     logging.info(f"Dumped: {meta_json}")
 
 
 if __name__ == "__main__":
```

### Comparing `pydtk-0.2.9/pydtk/bin/oas.py` & `pydtk-0.3.0/pydtk/bin/oas.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,23 @@
 
 class OpenAPISpecification(object):
     """Generate OpenAPI Specification."""
 
     def __init__(self, out_dir: str) -> None:
         assert os.path.isdir(out_dir), f"Directory '{out_dir}' is not found."
         self.out_dir = out_dir
-        self._schema_dir = os.path.join(
-            os.path.dirname(pydtk.__file__), "db", "schemas"
-        )
+        self._schema_dir = os.path.join(os.path.dirname(pydtk.__file__), "db", "schemas")
 
     def dump(self) -> None:
         """Dump OpenAPI Specification."""
         for rel_file_path, schemas in SCHEMAS_BY_FILES.items():
             rel_out_path = rel_file_path.replace(".py", ".json")
             self.dump_schemas_as_oas(schemas, rel_out_path, self.out_dir)
 
-    def dump_schemas_as_oas(
-        self, schemas: list, rel_out_path: str, output_dir: str
-    ) -> None:
+    def dump_schemas_as_oas(self, schemas: list, rel_out_path: str, output_dir: str) -> None:
         """Dump schema information in the form of OpenAPI Specification format.
 
         Args:
             schemas (list): List of target schemas.
             rel_out_path (str): Relative output path.
             output_dir (str): Output directory.
         """
```

### Comparing `pydtk-0.2.9/pydtk/bin/sub_commands/db.py` & `pydtk-0.3.0/pydtk/bin/sub_commands/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,26 +156,22 @@
             $ pydtk db list records --parsable
 
             ```
 
         """
         _assert_target(target)
 
-        handler, group_by = _get_db_handler(
-            target, database_id=database_id, base_dir=base_dir
-        )
+        handler, group_by = _get_db_handler(target, database_id=database_id, base_dir=base_dir)
 
         # Prepare search query
         if order_by is not None:
             order_by = [(order_by, 1)]
 
         # Read
-        handler.read(
-            pql=pql, limit=limit, offset=offset, order_by=order_by, group_by=group_by
-        )
+        handler.read(pql=pql, limit=limit, offset=offset, order_by=order_by, group_by=group_by)
 
         # Display
         _display(
             handler,
             columns=[
                 "Database ID",
                 "Record ID",
@@ -210,17 +206,15 @@
             path (str): File path
             content (str): Content
             base_dir (str): Base directory
 
         """
         _assert_target(target)
 
-        handler, group_by = _get_db_handler(
-            target, database_id=database_id, base_dir=base_dir
-        )
+        handler, group_by = _get_db_handler(target, database_id=database_id, base_dir=base_dir)
 
         # Prepare query
         pql = ""
         if target in ["database", "databases"]:
             if database_id is not None:
                 pql += " and " if pql != "" else ""
                 pql += 'database_id == "{}"'.format(database_id)
@@ -468,17 +462,15 @@
         return
     if "p" in kwargs and kwargs["p"]:
         parsable = True
     if "parsable" in kwargs and kwargs["parsable"]:
         parsable = True
 
     if not parsable:
-        available_columns = [
-            column for column in handler.df.columns if not column.startswith("_")
-        ]
+        available_columns = [column for column in handler.df.columns if not column.startswith("_")]
         if columns is not None:
             df = handler.df[[c for c in columns if c in available_columns]]
         else:
             df = handler.df[available_columns]
         if include_summary:
             print(f"Found: {handler.count_total} items.")
         if handler.count_total > len(handler):
```

### Comparing `pydtk-0.2.9/pydtk/bin/sub_commands/io.py` & `pydtk-0.3.0/pydtk/bin/sub_commands/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,10 @@
             file (str): Path to a file
             content (str): Content in the file to read
 
         """
         from pydtk.io import BaseFileReader
 
         reader = BaseFileReader()
-        timestamps, data, columns = reader.read(
-            path=file, contents=content, as_ndarray=False
-        )
+        timestamps, data, columns = reader.read(path=file, contents=content, as_ndarray=False)
 
         pprint.pprint(data)
```

### Comparing `pydtk-0.2.9/pydtk/bin/sub_commands/model.py` & `pydtk-0.3.0/pydtk/bin/sub_commands/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,15 @@
                 model = getattr(
                     importlib.import_module(".".join(model.split(".")[:-1])),
                     model.split(".")[-1],
                 )
 
             # Get contents and timestamps
             try:
-                data["contents"] = model.generate_contents_meta(
-                    path=from_file, content_key=content
-                )
+                data["contents"] = model.generate_contents_meta(path=from_file, content_key=content)
             except NotImplementedError:
                 pass
             try:
                 (
                     data["start_timestamp"],
                     data["end_timestamp"],
                 ) = model.generate_timestamp_meta(path=from_file)
```

### Comparing `pydtk-0.2.9/pydtk/bin/sub_commands/status.py` & `pydtk-0.3.0/pydtk/bin/sub_commands/status.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/builder/concat_df.py` & `pydtk-0.3.0/pydtk/builder/concat_df.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/builder/dbdb/file_info.py` & `pydtk-0.3.0/pydtk/builder/dbdb/file_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 
 
 def _read_timestamp(file):
     """Get start and end time from timestamp csv file."""
     try:
         with open(file, "r") as f:
             rows = f.readlines()
-            starttime, endtime = float(rows[0].split(",")[0]), float(
-                rows[-1].split(",")[0]
-            )
+            starttime, endtime = float(rows[0].split(",")[0]), float(rows[-1].split(",")[0])
         starttime, endtime = starttime / (10**3), endtime / (10**3)
     except IOError:
         starttime, endtime = "Nan", "Nan"
     return starttime, endtime
 
 
 def _get_time_info(file):
@@ -86,17 +84,15 @@
         contents[contents_name] = {"tags": contents_tags}
     elif file.endswith("bag"):
         bag_info = _read_rosbag(file)
         topic_info = bag_info["topic_info"]
         topics = [topic for topic in topic_info[1].keys()]
         topics.sort()
         for topic in topics:
-            if topic.startswith(
-                "/mobileye"
-            ):  # mobileye data is not supported at this version
+            if topic.startswith("/mobileye"):  # mobileye data is not supported at this version
                 continue
             contents[topic] = {}
             contents[topic]["msg_type"] = topic_info[1][topic].msg_type
             contents[topic]["msg_md5sum"] = topic_info[0][topic_info[1][topic].msg_type]
             contents[topic]["count"] = topic_info[1][topic].message_count
             contents[topic]["frequency"] = topic_info[1][topic].frequency
             contents[topic]["tags"] = re.split("[_/-]", topic[1:])
@@ -124,17 +120,15 @@
     attributes = OrderedDict()
 
     attributes["description"] = "Driving Database"
     attributes["database_id"] = "Driving Behavior Database"
     attributes["record_id"] = file_path.split("/")[-3]
     attributes["type"] = "raw_data"  # 収録データ
     attributes["path"] = file_path
-    attributes["start_timestamp"], attributes["end_timestamp"] = _get_time_info(
-        file_path
-    )
+    attributes["start_timestamp"], attributes["end_timestamp"] = _get_time_info(file_path)
 
     attributes["content-type"] = _check_content_type(file_path)
     attributes["contents"] = _check_contents(file_path)
 
     with open(json_path, mode="w") as f:
         json.dump(attributes, f, ensure_ascii=False, indent=4, separators=(",", ": "))
     logging.debug("Finish writing: %s" % json_path)
```

### Comparing `pydtk-0.2.9/pydtk/builder/df_list.py` & `pydtk-0.3.0/pydtk/builder/df_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,17 +186,15 @@
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="This script is bababa")
     parser.add_argument(
         "--db_dir",
         default="/data_pool_1/DrivingBehaviorDatabase/records",
         help="Path to database directory",
     )
-    parser.add_argument(
-        "--pkl", default="pydtk_DBDB.pkl", help="Pickle file path to save"
-    )
+    parser.add_argument("--pkl", default="pydtk_DBDB.pkl", help="Pickle file path to save")
     parser.add_argument("--start", default=0, type=int, help="Start HDD ID for index")
     parser.add_argument("--end", default=999, type=int, help="End HDD ID for index")
     parser.add_argument("-v", "--verbose", action="store_true", help="Verbose mode")
 
     args = parser.parse_args()
 
     if args.verbose:
```

### Comparing `pydtk-0.2.9/pydtk/builder/df_path.py` & `pydtk-0.3.0/pydtk/builder/df_path.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/builder/meta_db.py` & `pydtk-0.3.0/pydtk/builder/meta_db.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/builder/statistic_db.py` & `pydtk-0.3.0/pydtk/builder/statistic_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,17 +186,15 @@
         stat_db_handler.df = stat_df
         stat_db_handler.save()
 
     tqdm.pandas(desc="Load files, calculate and write")
     for sample in meta_db_handler:
         write_stat_to_db(sample)
     t_n, t_p = time.time(), t_n
-    logging.info(
-        "Calculated statistics and wrote to DB.({0:.03f} secs)".format(t_n - t_p)
-    )
+    logging.info("Calculated statistics and wrote to DB.({0:.03f} secs)".format(t_n - t_p))
 
     logging.info("Done.(Total: {0:.03f} secs)".format(t_n - t_b))
 
 
 def batch_script():
     """Function for tool.poetry.scripts."""
     fire.Fire(batch_analysis)
```

### Comparing `pydtk-0.2.9/pydtk/conf/v1.yaml` & `pydtk-0.3.0/pydtk/conf/v1.yaml`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/conf/v2.yaml` & `pydtk-0.3.0/pydtk/conf/v2.yaml`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/conf/v3.yaml` & `pydtk-0.3.0/pydtk/conf/v3.yaml`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/conf/v4.yaml` & `pydtk-0.3.0/pydtk/conf/v4.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
       database: ""
     statistics:
       engine: tinymongo
       host: /tmp/pydtk-statistics
       username: ""
       password: ""
       database: ""
-    annotations:
+    annotation:
       engine: tinymongo
       host: /tmp/pydtk-annotations
       username: ""
       password: ""
       database: ""
 
   df_class:
@@ -75,14 +75,22 @@
           dtype: string
           aggregation: push
           display_name: File path
         - name: contents
           dtype: dict
           aggregation: mergeObjects
           display_name: Contents
+        - name: start_timestamp
+          dtype: float
+          aggregation: min
+          display_name: Start timestamp
+        - name: end_timestamp
+          dtype: float
+          aggregation: max
+          display_name: End timestamp
       index_columns:
         - _kind
         - record_id
         - path
     time_series_df:
       index_columns:
         - record_id
```

### Comparing `pydtk-0.2.9/pydtk/db/__init__.py` & `pydtk-0.3.0/pydtk/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/schemas/__init__.py` & `pydtk-0.3.0/pydtk/db/schemas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,15 @@
             for prop, value in schema.get("properties", {}).items():
                 # retrieve right field from alias or name
                 field = [x for x in model.__fields__.values() if x.alias == prop][0]
                 if field.allow_none:
                     if "$ref" in value:
                         if issubclass(field.type_, BaseSchema):
                             # add 'title' in schema to have the exact same behaviour as the rest
-                            value["title"] = (
-                                field.type_.__config__.title or field.type_.__name__
-                            )
+                            value["title"] = field.type_.__config__.title or field.type_.__name__
                         value["anyOf"] = [{"$ref": value.pop("$ref")}]
 
                     value["nullable"] = True
 
 
 def get_schema(api_version: str, kind: str):
     """Get schema based on the given `api_version` and `kind`.
@@ -115,16 +113,14 @@
         kind (str): Kind of information.
 
     Returns:
         (BaseSchema): the corresponding schema.
 
     """
     try:
-        schema = SCHEMAS_BY_VERSIONS[api_version.replace("/", os.sep).lower()][
-            kind.lower()
-        ]
+        schema = SCHEMAS_BY_VERSIONS[api_version.replace("/", os.sep).lower()][kind.lower()]
     except KeyError:
         raise SchemaNotFoundError()
     return schema
 
 
 register_schemas()
```

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_pixel.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha5/annotation_commented_image_pixel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,34 @@
+import os
+
 from pydantic import BaseModel, Field, constr
 
 from pydtk.db.schemas import register_schema
+from pydtk.utils.imports import import_module_from_path
 
-try:
-    # NOTE(kan-bayashi): absolute and relative path import does not work
-    from annotation import Annotation
-except ImportError:
-    import os
-    import sys
-
-    sys.path.append(os.path.dirname(__file__))
-    from annotation import Annotation
+annotation = import_module_from_path(f"{os.path.dirname(__file__)}/annotation.py")
 
 
 class ImagePixel(BaseModel):
     """Schema for image pixel."""
 
-    x: int
-    y: int
+    x: float
+    y: float
 
 
 class CommentedImagePixel(BaseModel):
     """Schema for commented image pixel."""
 
     text: constr(min_length=1) = Field(..., description="")
     # NOTE(kan-bayashi): Sometimes frame_id in image message is empty.
     frame_id: constr(min_length=0) = Field(..., description="Cordinate ID.")
-    target_topic: constr(min_length=1) = Field(
-        ..., description="Target topic to comment."
-    )
+    target_topic: constr(min_length=1) = Field(..., description="Target topic to comment.")
     image_pixel: ImagePixel
 
 
 @register_schema
-class AnnotationCommentedImagePixel(Annotation):
+class AnnotationCommentedImagePixel(annotation.Annotation):
     """Schema for commented image pixel annotation."""
 
-    _api_version = "dataware-tools.com/v1alpha1"
+    _api_version = "dataware-tools.com/v1alpha5"
     _kind = "AnnotationCommentedImagePixel"
     commented_image_pixel: CommentedImagePixel
```

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_rectangular_area.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_rectangular_area.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,15 @@
+import os
+
 from pydantic import BaseModel, Field, constr
 
 from pydtk.db.schemas import register_schema
+from pydtk.utils.imports import import_module_from_path
 
-try:
-    # NOTE(kan-bayashi): absolute and relative path import does not work
-    from annotation import Annotation
-except ImportError:
-    import os
-    import sys
-
-    sys.path.append(os.path.dirname(__file__))
-    from annotation import Annotation
+annotation = import_module_from_path(f"{os.path.dirname(__file__)}/annotation.py")
 
 
 class ImageRectangularArea(BaseModel):
     """Schema for image rectangular area."""
 
     # TODO(kan-bayashi): Check frontend side
     # TODO(kan-bayashi): Add cordinate figure in docstrings
@@ -26,20 +21,18 @@
 
 class CommentedImageRectangularArea(BaseModel):
     """Schema for commented image rectangular area."""
 
     text: constr(min_length=1) = Field(..., description="")
     # NOTE(kan-bayashi): Sometimes frame_id in image message is empty.
     frame_id: constr(min_length=0) = Field(..., description="Cordinate ID.")
-    target_topic: constr(min_length=1) = Field(
-        ..., description="Target topic to comment."
-    )
+    target_topic: constr(min_length=1) = Field(..., description="Target topic to comment.")
     image_rectangular_area: ImageRectangularArea
 
 
 @register_schema
-class AnnotationCommentedImageRectanglerArea(Annotation):
+class AnnotationCommentedImageRectanglerArea(annotation.Annotation):
     """Schema for commented image rectangular area annotation."""
 
-    _api_version = "dataware-tools.com/v1alpha1"
+    _api_version = "dataware-tools.com/v1alpha2"
     _kind = "AnnotationCommentedImageRectanglerArea"
     commented_image_rectangular_area: CommentedImageRectangularArea
```

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_point.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_point.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,15 @@
+import os
+
 from pydantic import BaseModel, Field, constr
 
 from pydtk.db.schemas import register_schema
+from pydtk.utils.imports import import_module_from_path
 
-try:
-    # NOTE(kan-bayashi): absolute and relative path import does not work
-    from annotation import Annotation
-except ImportError:
-    import os
-    import sys
-
-    sys.path.append(os.path.dirname(__file__))
-    from annotation import Annotation
+annotation = import_module_from_path(f"{os.path.dirname(__file__)}/annotation.py")
 
 
 class Point(BaseModel):
     """Schema for point."""
 
     x: float
     y: float
@@ -26,13 +21,13 @@
 
     text: constr(min_length=1) = Field(..., description="")
     frame_id: constr(min_length=1) = Field(..., description="Cordinate ID.")
     point: Point
 
 
 @register_schema
-class AnnotationCommentedPoint(Annotation):
+class AnnotationCommentedPoint(annotation.Annotation):
     """Schema for commented point annotation."""
 
-    _api_version = "dataware-tools.com/v1alpha1"
+    _api_version = "dataware-tools.com/v1alpha2"
     _kind = "AnnotationCommentedPoint"
     commented_point: CommentedPoint
```

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/file.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha1/file.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from pydantic import Field, constr
 from typing import Union
 
+from pydantic import Field, constr
+
 from pydtk.db.schemas import BaseSchema, register_schema
 
 
 @register_schema
 class Annotation(BaseSchema):
     """Schema for annotation."""
```

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_pixel.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha4/annotation_commented_image_pixel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,15 @@
+import os
+
 from pydantic import BaseModel, Field, constr
 
 from pydtk.db.schemas import register_schema
+from pydtk.utils.imports import import_module_from_path
 
-try:
-    # NOTE(kan-bayashi): absolute and relative path import does not work
-    from annotation import Annotation
-except ImportError:
-    import os
-    import sys
-
-    sys.path.append(os.path.dirname(__file__))
-    from annotation import Annotation
+annotation = import_module_from_path(f"{os.path.dirname(__file__)}/annotation.py")
 
 
 class ImagePixel(BaseModel):
     """Schema for image pixel."""
 
     x: int
     y: int
@@ -22,20 +17,18 @@
 
 class CommentedImagePixel(BaseModel):
     """Schema for commented image pixel."""
 
     text: constr(min_length=1) = Field(..., description="")
     # NOTE(kan-bayashi): Sometimes frame_id in image message is empty.
     frame_id: constr(min_length=0) = Field(..., description="Cordinate ID.")
-    target_topic: constr(min_length=1) = Field(
-        ..., description="Target topic to comment."
-    )
+    target_topic: constr(min_length=1) = Field(..., description="Target topic to comment.")
     image_pixel: ImagePixel
 
 
 @register_schema
-class AnnotationCommentedImagePixel(Annotation):
+class AnnotationCommentedImagePixel(annotation.Annotation):
     """Schema for commented image pixel annotation."""
 
-    _api_version = "dataware-tools.com/v1alpha2"
+    _api_version = "dataware-tools.com/v1alpha4"
     _kind = "AnnotationCommentedImagePixel"
     commented_image_pixel: CommentedImagePixel
```

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_rectangular_area.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/annotation_commented_image_rectangular_area.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,15 @@
+import os
+
 from pydantic import BaseModel, Field, constr
 
 from pydtk.db.schemas import register_schema
+from pydtk.utils.imports import import_module_from_path
 
-try:
-    # NOTE(kan-bayashi): absolute and relative path import does not work
-    from annotation import Annotation
-except ImportError:
-    import os
-    import sys
-
-    sys.path.append(os.path.dirname(__file__))
-    from annotation import Annotation
+annotation = import_module_from_path(f"{os.path.dirname(__file__)}/annotation.py")
 
 
 class ImageRectangularArea(BaseModel):
     """Schema for image rectangular area."""
 
     # TODO(kan-bayashi): Check frontend side
     # TODO(kan-bayashi): Add cordinate figure in docstrings
@@ -26,20 +21,18 @@
 
 class CommentedImageRectangularArea(BaseModel):
     """Schema for commented image rectangular area."""
 
     text: constr(min_length=1) = Field(..., description="")
     # NOTE(kan-bayashi): Sometimes frame_id in image message is empty.
     frame_id: constr(min_length=0) = Field(..., description="Cordinate ID.")
-    target_topic: constr(min_length=1) = Field(
-        ..., description="Target topic to comment."
-    )
+    target_topic: constr(min_length=1) = Field(..., description="Target topic to comment.")
     image_rectangular_area: ImageRectangularArea
 
 
 @register_schema
-class AnnotationCommentedImageRectanglerArea(Annotation):
+class AnnotationCommentedImageRectangularArea(annotation.Annotation):
     """Schema for commented image rectangular area annotation."""
 
-    _api_version = "dataware-tools.com/v1alpha2"
-    _kind = "AnnotationCommentedImageRectanglerArea"
+    _api_version = "dataware-tools.com/v1alpha3"
+    _kind = "AnnotationCommentedImageRectangularArea"
     commented_image_rectangular_area: CommentedImageRectangularArea
```

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/file.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha2/record.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from typing import Optional, Dict, Any, Type
+from typing import Any, Dict, Optional, Type
 
-from pydantic import Field, constr, Extra
+from pydantic import Extra, Field, constr
 
 from pydtk.db.schemas import BaseSchema, register_schema
 
 
 @register_schema
-class File(BaseSchema):
-    """Schema for files."""
+class Record(BaseSchema):
+    """Schema for records."""
 
     _api_version = "dataware-tools.com/v1alpha2"
-    _kind = "File"
+    _kind = "Record"
     description: Optional[constr()] = Field(None, description="")
     record_id: constr(min_length=1) = Field(..., description="")
-    path: constr(min_length=1) = Field(..., description="")
-    contents: Optional[dict] = Field(None, description="")
 
     # Allow additional properties
     class Config(BaseSchema.Config):
         """Config."""
 
         extra = Extra.allow
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any], model: Type['File']):
+        def schema_extra(schema: Dict[str, Any], model: Type["Record"]):
             """Extra schema."""
             BaseSchema.Config.schema_extra(schema, model)
             schema["additionalProperties"] = {}
```

### Comparing `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/record.py` & `pydtk-0.3.0/pydtk/db/schemas/dataware-tools.com/v1alpha3/record.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Optional, Dict, Any, Type
+from typing import Any, Dict, Optional, Type
 
-from pydantic import Field, constr, Extra
+from pydantic import Extra, Field, constr
 
 from pydtk.db.schemas import BaseSchema, register_schema
 
 
 @register_schema
 class Record(BaseSchema):
     """Schema for records."""
 
-    _api_version = "dataware-tools.com/v1alpha2"
+    _api_version = "dataware-tools.com/v1alpha3"
     _kind = "Record"
     description: Optional[constr()] = Field(None, description="")
     record_id: constr(min_length=1) = Field(..., description="")
 
     # Allow additional properties
     class Config(BaseSchema.Config):
         """Config."""
 
         extra = Extra.allow
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any], model: Type['Record']):
+        def schema_extra(schema: Dict[str, Any], model: Type["Record"]):
             """Extra schema."""
             BaseSchema.Config.schema_extra(schema, model)
             schema["additionalProperties"] = {}
```

### Comparing `pydtk-0.2.9/pydtk/db/v1/handlers/__init__.py` & `pydtk-0.3.0/pydtk/db/v1/handlers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,17 +168,15 @@
         if self._df is None:
             self._df = vaex.from_dict(data)
         else:
             if check_unique:
                 # TODO(hdl-members): support unique-check for multiple items
                 df_uuid = data["uuid_in_df"][0]
                 if len(self.df[self.df.uuid_in_df.str.equals(df_uuid)]) > 0:
-                    logging.warning(
-                        "Given data already exist in dataframe: {}".format(df_uuid)
-                    )
+                    logging.warning("Given data already exist in dataframe: {}".format(df_uuid))
                     return
             self.df = self.df.concat(vaex.from_dict(data))
 
     def add_data(self, data_in, **kwargs):
         """Add data to db.
 
         Args:
```

### Comparing `pydtk-0.2.9/pydtk/db/v1/handlers/meta.py` & `pydtk-0.3.0/pydtk/db/v1/handlers/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,15 @@
         if "path" in data_in.keys():
             # noinspection PyTypeChecker
             data_path = Path(data_in["path"])
             try:
                 relative_path = data_path.relative_to(self.base_dir_path)
                 data_in["path"] = relative_path
             except ValueError as e:
-                logging.warning(
-                    "Could not resolve relative path to file: {}".format(data_path)
-                )
+                logging.warning("Could not resolve relative path to file: {}".format(data_path))
                 logging.warning(str(e))
 
         # Parse contents
         data_out = []
         for content_name, content_info in data_in["contents"].items():
             data = deepcopy(data_in)
             data["content"] = content_name
```

### Comparing `pydtk-0.2.9/pydtk/db/v2/handlers/__init__.py` & `pydtk-0.3.0/pydtk/db/v2/handlers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,17 +150,15 @@
         if engine in ["influxdb"]:
             if not _extra_supports["influxdb"]:
                 raise ImportError("Module `influxdb` cannot be not imported")
             hostname = host
             hostport = 8086
             if ":" in host:
                 hostname, hostport = host.split(":")
-            self._engine = DataFrameClient(
-                hostname, hostport, username, password, database
-            )
+            self._engine = DataFrameClient(hostname, hostport, username, password, database)
         else:
             engine = (
                 "postgresql"
                 if engine == "timescaledb"
                 else "mysql"
                 if engine == "mariadb"
                 else engine
@@ -181,17 +179,15 @@
             )
             self._session = scoped_session(sessionmaker(bind=self._engine))
 
     def _initialize_df(self):
         """Initialize DF."""
         df = pd.concat(
             [
-                pd.Series(
-                    name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"])
-                )
+                pd.Series(name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"]))
                 for c in self.columns
             ]
             + [pd.Series(name="uuid_in_df", dtype=str)],
             axis=1,
         )
         return df
 
@@ -356,17 +352,15 @@
         try:
             if self._config.current_db["engine"] in ["influxdb"]:
                 df = list(self._engine.query(str(q), **kwargs).values())[0]
             else:
                 df = pd.read_sql_query(q, self._engine, **kwargs)
         except Exception as e:
             self.logger.warning(
-                'Could not execute SQL statement: "{0}" (reason: {1})'.format(
-                    str(q), str(e)
-                )
+                'Could not execute SQL statement: "{0}" (reason: {1})'.format(str(q), str(e))
             )
             df = self._initialize_df()
 
         self.df = df
 
     def save(self, df=None, remove_duplicates=False, **kwargs):
         """Save data to SQL.
@@ -404,62 +398,50 @@
                 select = 'select distinct * from "{0}"'.format(self.df_name)
             else:
                 raise ValueError("Unsupported engine: {}".format(self._engine.name))
             q = 'insert into "{0}" {1}'.format(temp_table_name, select)
             self._engine.execute(q)
 
             # Drop deprecated table if exists
-            if self._engine.dialect.has_table(
-                self._engine, self.df_name + "_deprecated"
-            ):
-                self._engine.execute(
-                    'drop table "{0}"'.format(self.df_name + "_deprecated")
-                )
+            if self._engine.dialect.has_table(self._engine, self.df_name + "_deprecated"):
+                self._engine.execute('drop table "{0}"'.format(self.df_name + "_deprecated"))
 
             # Deprecate the original table
             self._engine.execute(
                 'alter table "{0}" rename to "{1}"'.format(
                     self.df_name, self.df_name + "_deprecated"
                 )
             )
 
             # Rename the temporal table
             self._engine.execute(
-                'alter table "{0}" rename to "{1}"'.format(
-                    temp_table_name, self.df_name
-                )
+                'alter table "{0}" rename to "{1}"'.format(temp_table_name, self.df_name)
             )
 
             # Drop the deprecated table
-            self._engine.execute(
-                'drop table "{0}"'.format(self.df_name + "_deprecated")
-            )
+            self._engine.execute('drop table "{0}"'.format(self.df_name + "_deprecated"))
 
     @property
     def df(self):
         """Return df."""
         return self._df
 
     @df.setter
     def df(self, value):
         """Setter for self.df."""
         if not isinstance(value, pd.DataFrame):
             raise ValueError("Only pandas dataframe is accepted.")
 
         # Set columns based on the given DF
         if len(self.columns) == 0 and len(value) > 0:
-            self.columns = [
-                {"name": c, "dtype": "none"} for c in value.columns.to_list()
-            ]
+            self.columns = [{"name": c, "dtype": "none"} for c in value.columns.to_list()]
 
         # Add column 'uuid_in_df'
         if "uuid_in_df" not in value.columns.to_list():
-            value["uuid_in_df"] = value.apply(
-                lambda x: self._get_uuid_from_item(x), axis=1
-            )
+            value["uuid_in_df"] = value.apply(lambda x: self._get_uuid_from_item(x), axis=1)
             self.columns += [{"name": "uuid_in_df", "dtype": "str"}]
 
         self._df = value
 
     @property
     def df_name(self):
         """Return df_name."""
@@ -480,34 +462,28 @@
         except KeyError:
             return []
 
     @columns.setter
     def columns(self, value):
         """Set self.columns."""
         if not isinstance(value, list):
-            raise ValueError(
-                'Columns must be a list of dicts with keys "name" and "dtype".'
-            )
+            raise ValueError('Columns must be a list of dicts with keys "name" and "dtype".')
         if len(value) < 1:
             raise ValueError("At least one item must be in the list.")
         if (
             not isinstance(value[0], dict)
             or "name" not in value[0].keys()
             or "dtype" not in value[0].keys()
         ):
-            raise ValueError(
-                'Columns must be a list of dicts with keys "name" and "dtype".'
-            )
+            raise ValueError('Columns must be a list of dicts with keys "name" and "dtype".')
 
         try:
             _ = pd.concat(
                 [
-                    pd.Series(
-                        name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"])
-                    )
+                    pd.Series(name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"]))
                     for c in value
                 ]
                 + [pd.Series(name="uuid_in_df", dtype=str)],
                 axis=1,
             )
         except KeyError as e:
             raise ValueError("Unrecognized value: {}".format(str(e)))
@@ -560,16 +536,14 @@
 
         """
         dataframe: pd.DataFrame = df if df is not None else self.df
 
         # Convert timestamp (float) to datetime
         assert "timestamp" in dataframe.columns
         df_to_save = dataframe.copy()
-        df_to_save["timestamp"] = pd.to_datetime(
-            df_to_save["timestamp"].astype(float), unit="s"
-        )
+        df_to_save["timestamp"] = pd.to_datetime(df_to_save["timestamp"].astype(float), unit="s")
         df_to_save.set_index("timestamp", inplace=True)
 
         if self._config.current_db["engine"] in ["influxdb"]:
             super().save(df=df_to_save)
         else:
             super().save(df=df_to_save, index=True)
```

### Comparing `pydtk-0.2.9/pydtk/db/v2/handlers/meta.py` & `pydtk-0.3.0/pydtk/db/v2/handlers/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,15 @@
         if "path" in data_in.keys():
             # noinspection PyTypeChecker
             data_path = Path(data_in["path"])
             try:
                 relative_path = data_path.relative_to(self.base_dir_path)
                 data_in["path"] = relative_path
             except ValueError as e:
-                logging.warning(
-                    "Could not resolve relative path to file: {}".format(data_path)
-                )
+                logging.warning("Could not resolve relative path to file: {}".format(data_path))
                 logging.warning(str(e))
 
         # Parse contents
         data_out = []
         for content_name, content_info in data_in["contents"].items():
             data = deepcopy(data_in)
             data["contents"] = content_name
```

### Comparing `pydtk-0.2.9/pydtk/db/v2/search_engines/__init__.py` & `pydtk-0.3.0/pydtk/db/v2/search_engines/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v2/search_engines/time_series.py` & `pydtk-0.3.0/pydtk/db/v2/search_engines/time_series.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v3/__init__.py` & `pydtk-0.3.0/pydtk/db/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v3/handlers/__init__.py` & `pydtk-0.3.0/pydtk/db/v3/handlers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,17 +68,17 @@
         if not os.path.isfile(os.path.join(os.path.dirname(__file__), filename)):
             continue
         if filename == "__init__.py":
             continue
 
         try:
             importlib.import_module(
-                os.path.join(
-                    "pydtk.db.v3.handlers", os.path.splitext(filename)[0]
-                ).replace(os.sep, ".")
+                os.path.join("pydtk.db.v3.handlers", os.path.splitext(filename)[0]).replace(
+                    os.sep, "."
+                )
             )
         except ModuleNotFoundError:
             logging.debug("Failed to load handlers in {}".format(filename))
 
 
 def register_handler(db_classes, db_engines):
     """Register a DB-handler.
@@ -142,17 +142,15 @@
 
         # Check if the db_class is available
         if db_class not in DB_HANDLERS.keys():
             raise ValueError("Unsupported db_class: {}".format(db_class))
 
         # Get db_engine from environment variable if not specified
         if db_engine is None:
-            db_engine = os.environ.get(
-                "PYDTK_{}_DB_ENGINE".format(db_class.upper()), None
-            )
+            db_engine = os.environ.get("PYDTK_{}_DB_ENGINE".format(db_class.upper()), None)
 
         # Get the default engine if not specified
         if db_engine is None:
             try:
                 db_defaults = getattr(config.sql, db_class)
                 db_engine = db_defaults.engine
             except (ValueError, AttributeError):
@@ -200,17 +198,15 @@
 
         return data
 
     def _initialize_df(self):
         """Initialize DF."""
         df = pd.concat(
             [
-                pd.Series(
-                    name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"])
-                )
+                pd.Series(name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"]))
                 for c in self.columns
                 if c["name"] != "uuid_in_df" and c["name"] != "creation_time_in_df"
             ]  # noqa: E501
             + [
                 pd.Series(name="uuid_in_df", dtype=str),
                 pd.Series(name="creation_time_in_df", dtype=float),
             ],
@@ -346,51 +342,39 @@
 
         """
         if df_name is not None:
             self.df_name = df_name
 
         # Create a query
         q = query
-        q_count = (
-            "select count(*) from ({}) as sub".format(q) if q is not None else None
-        )
+        q_count = "select count(*) from ({}) as sub".format(q) if q is not None else None
         if q is None:
             # Check if the table exits on DB
             if not inspect(self._engine).has_table(self.df_name):
                 self.df = self._initialize_df()
                 return
 
             # Create a query
             if self._config.current_db["engine"] in ["postgresql", "timescaledb"]:
                 q = sql.select("*", from_obj=sql.table(self.df_name))
                 if group_by is not None:
                     q = sql.select(
-                        [
-                            sql.text(self._distinct(c))
-                            for c in self._get_column_names_from_db()
-                        ],
+                        [sql.text(self._distinct(c)) for c in self._get_column_names_from_db()],
                         from_obj=sql.table(self.df_name),
                     )
                     q = q.group_by(sql.text(group_by))
                 if where is not None:
                     q = q.where(sql.text(where))
-                q_count = sql.select(
-                    [sql.text("count(*)")], from_obj=sql.alias(q, "sub")
-                )
+                q_count = sql.select([sql.text("count(*)")], from_obj=sql.alias(q, "sub"))
             else:
                 q = sql.select("*", from_obj=sql.table(self.df_name))
-                q_count = sql.select(
-                    [sql.text("count(*)")], from_obj=sql.table(self.df_name)
-                )
+                q_count = sql.select([sql.text("count(*)")], from_obj=sql.table(self.df_name))
                 if group_by is not None:
                     q = sql.select(
-                        [
-                            sql.text(self._distinct(c))
-                            for c in self._get_column_names_from_db()
-                        ],
+                        [sql.text(self._distinct(c)) for c in self._get_column_names_from_db()],
                         from_obj=sql.table(self.df_name),
                     )
                     q = q.group_by(sql.text(group_by))
                     q_count = sql.select(
                         [sql.text("count(distinct {})".format(group_by))],
                         from_obj=sql.table(self.df_name),
                     )
@@ -417,17 +401,15 @@
             # Fetch data
             if "index_col" not in kwargs.keys():
                 kwargs.update({"index_col": "uuid_in_df"})
             df = pd.read_sql_query(q, self._engine, **kwargs)
             df = df[~df.index.duplicated(keep="last")]
         except Exception as e:
             self.logger.warning(
-                'Could not execute SQL statement: "{0}" (reason: {1})'.format(
-                    str(q), str(e)
-                )
+                'Could not execute SQL statement: "{0}" (reason: {1})'.format(str(q), str(e))
             )
             count = 0
             df = self._initialize_df()
 
         self._count_total = count
         self.df = df
 
@@ -464,29 +446,23 @@
             return
 
         # Get table
         meta = MetaData(bind=self._engine)
         table = Table(self.df_name, meta, autoload=True)
 
         # Add columns
-        for column_name in set([c["name"] for c in self.columns]).difference(
-            existing_columns
-        ):
+        for column_name in set([c["name"] for c in self.columns]).difference(existing_columns):
             column = next((filter(lambda c: c["name"] == column_name, self.columns)))
             column_name = column["name"]
             if column_name in ["uuid_in_df"]:
                 column_dtype = VARCHAR(32)
             elif column_name in ["creation_time_in_df"]:
-                column_dtype = map_dtype("double", self._config.current_db["engine"])[
-                    "sql"
-                ]
+                column_dtype = map_dtype("double", self._config.current_db["engine"])["sql"]
             else:
-                column_dtype = map_dtype(
-                    column["dtype"], self._config.current_db["engine"]
-                )["sql"]
+                column_dtype = map_dtype(column["dtype"], self._config.current_db["engine"])["sql"]
             create_column(Column(column_name, column_dtype), table)
 
     def _quote(self, value):
         if self._config.current_db["engine"] in ["mariadb"]:
             return "`{}`".format(value)
         else:
             return '"{}"'.format(value)
@@ -499,17 +475,15 @@
 
         Returns:
             (str): selection key
 
         """
         column_dtype = None
         if column_name in self._get_column_names():
-            column_info = next(
-                iter(filter(lambda c: c["name"] == column_name, self.columns))
-            )
+            column_info = next(iter(filter(lambda c: c["name"] == column_name, self.columns)))
             column_dtype = column_info["dtype"]
 
         if self._config.current_db["engine"] in ["postgresql", "timescaledb"]:
             if column_dtype in ["string[]"]:
                 return "string_agg({0}, ';') as {0}".format(column_name)
             return "min({0}) as {0}".format(column_name)
         else:
@@ -535,34 +509,28 @@
                 ",".join([self._distinct(self._quote(c)) for c in columns]),
             )
         )
         self._engine.execute(q)
 
         # Create index
         if self._config.current_db["engine"] in ["sqlite"]:
-            q = "create index index_uuid_in_df on {} (uuid_in_df)".format(
-                self._quote(self.df_name)
-            )
+            q = "create index index_uuid_in_df on {} (uuid_in_df)".format(self._quote(self.df_name))
         elif self._config.current_db["engine"] in ["mysql", "mariadb"]:
             q = "alter table {} add index index_uuid_in_df(uuid_in_df)".format(
                 self._quote(self.df_name)
             )
         elif self._config.current_db["engine"] in ["postgresql", "timescaledb"]:
             q = "create index on {} (uuid_in_df)".format(self._quote(self.df_name))
         else:
-            raise ValueError(
-                "Unsupported engine: {}".format(self._config.current_db["engine"])
-            )
+            raise ValueError("Unsupported engine: {}".format(self._config.current_db["engine"]))
         self._engine.execute(q)
 
         # Drop deprecated table if exists
         if inspect(self._engine).has_table(self.df_name + "_deprecated"):
-            self._engine.execute(
-                "drop table {0}".format(self._quote(self.df_name + "_deprecated"))
-            )
+            self._engine.execute("drop table {0}".format(self._quote(self.df_name + "_deprecated")))
 
         # Deprecate the original table
         self._engine.execute(
             "alter table {0} rename to {1}".format(
                 self._quote(self.df_name), self._quote(self.df_name + "_deprecated")
             )
         )
@@ -571,17 +539,15 @@
         self._engine.execute(
             "alter table {0} rename to {1}".format(
                 self._quote(temp_table_name), self._quote(self.df_name)
             )
         )
 
         # Drop the deprecated table and temporal table
-        self._engine.execute(
-            "drop table {0}".format(self._quote(self.df_name + "_deprecated"))
-        )
+        self._engine.execute("drop table {0}".format(self._quote(self.df_name + "_deprecated")))
 
     @property
     def columns(self):
         """Return columns of DF."""
         if self._columns is not None:
             return self._columns
         try:
@@ -589,34 +555,28 @@
         except KeyError:
             return []
 
     @columns.setter
     def columns(self, value):
         """Set self.columns."""
         if not isinstance(value, list):
-            raise ValueError(
-                'Columns must be a list of dicts with keys "name" and "dtype".'
-            )
+            raise ValueError('Columns must be a list of dicts with keys "name" and "dtype".')
         if len(value) < 1:
             raise ValueError("At least one item must be in the list.")
         if (
             not isinstance(value[0], dict)
             or "name" not in value[0].keys()
             or "dtype" not in value[0].keys()
         ):
-            raise ValueError(
-                'Columns must be a list of dicts with keys "name" and "dtype".'
-            )
+            raise ValueError('Columns must be a list of dicts with keys "name" and "dtype".')
 
         try:
             _ = pd.concat(
                 [
-                    pd.Series(
-                        name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"])
-                    )
+                    pd.Series(name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"]))
                     for c in value
                 ]
                 + [
                     pd.Series(name="uuid_in_df", dtype=str),
                     pd.Series(name="creation_time_in_df", dtype=float),
                 ],
                 axis=1,
@@ -638,28 +598,24 @@
             raise ValueError("Only pandas dataframe is accepted.")
 
         if len(value) > 0:
             # Set columns based on the given DF
             self.columns = [
                 {
                     "name": c,
-                    "dtype": map_dtype(dtype.name, self._config.current_db["engine"])[
-                        "df"
-                    ],
+                    "dtype": map_dtype(dtype.name, self._config.current_db["engine"])["df"],
                 }
                 for c, dtype in value.dtypes.to_dict().items()
             ]
 
             # Add column 'uuid_in_df' and 'creation_time_in_df'
             if "uuid_in_df" not in self._get_column_names():
                 self.columns += [{"name": "uuid_in_df", "dtype": "str"}]
             if "uuid_in_df" not in value.columns.to_list():
-                value["uuid_in_df"] = value.apply(
-                    lambda x: self._get_uuid_from_item(x), axis=1
-                )
+                value["uuid_in_df"] = value.apply(lambda x: self._get_uuid_from_item(x), axis=1)
             if "creation_time_in_df" not in self._get_column_names():
                 self.columns += [{"name": "creation_time_in_df", "dtype": "double"}]
             if "creation_time_in_df" not in value.columns.to_list():
                 value["creation_time_in_df"] = datetime.now().timestamp()
             value.set_index("uuid_in_df", inplace=True)
 
         self._df = value
```

### Comparing `pydtk-0.2.9/pydtk/db/v3/handlers/meta.py` & `pydtk-0.3.0/pydtk/db/v3/handlers/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
 from tqdm import tqdm
 
 from . import BaseDBHandler as _BaseDBHandler
 from . import register_handler
 
 
-@register_handler(
-    db_classes=["meta"], db_engines=["sqlite", "mysql", "mariadb", "postgresql"]
-)
+@register_handler(db_classes=["meta"], db_engines=["sqlite", "mysql", "mariadb", "postgresql"])
 class MetaDBHandler(_BaseDBHandler):
     """Handler for metadb."""
 
     _database_id: str = ""
     _df_class = "meta_df"
     _df_name = "meta_df"
 
@@ -42,52 +40,42 @@
             if self._config.current_db["engine"] == "sqlite":
                 base_dir = os.path.dirname(self._config.current_db["host"])
             else:
                 base_dir = "/"
         self.base_dir_path = os.path.realpath(base_dir)
 
         # Prepare another DB-handler for storing a list of database_id
-        self._database_id_db_handler = DatabaseIDDBHandler(
-            **{**kwargs, "read_on_init": False}
-        )
+        self._database_id_db_handler = DatabaseIDDBHandler(**{**kwargs, "read_on_init": False})
 
     def _initialize_engine(
         self,
         db_engine=None,
         db_host=None,
         db_name=None,
         db_username=None,
         db_password=None,
     ):
         """Initialize DB engine."""
         # Load settings from environment variables
         engine = (
-            db_engine
-            if db_engine is not None
-            else os.environ.get("PYDTK_META_DB_ENGINE", None)
+            db_engine if db_engine is not None else os.environ.get("PYDTK_META_DB_ENGINE", None)
         )
         username = (
             db_username
             if db_username is not None
             else os.environ.get("PYDTK_META_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_META_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_META_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_META_DB_HOST", None)
         database = (
-            db_name
-            if db_name is not None
-            else os.environ.get("PYDTK_META_DB_DATABASE", None)
+            db_name if db_name is not None else os.environ.get("PYDTK_META_DB_DATABASE", None)
         )
 
         super()._initialize_engine(engine, host, database, username, password)
 
     def _serialize_contents_and_solve_path(self, data_in):
         """Serialize contents and fix absolute path to relative one.
 
@@ -107,29 +95,25 @@
         if "path" in data_in.keys():
             # noinspection PyTypeChecker
             data_path = Path(data_in["path"])
             try:
                 relative_path = data_path.relative_to(self.base_dir_path)
                 data_in["path"] = relative_path
             except ValueError as e:
-                logging.warning(
-                    "Could not resolve relative path to file: {}".format(data_path)
-                )
+                logging.warning("Could not resolve relative path to file: {}".format(data_path))
                 logging.warning(str(e))
 
         # Serialize contents
         data_out = []
         for content_name, content_info in data_in["contents"].items():
             for column_name in content_info.keys():
                 if column_name not in content_columns:
                     raise KeyError(
                         'Unrecognized key "{0}" found in content "{1}".'
-                        "  Please check the config file".format(
-                            column_name, content_name
-                        )
+                        "  Please check the config file".format(column_name, content_name)
                     )
             data = deepcopy(data_in)
             data["contents"] = content_name
             data.update(content_info)
             data_out.append(data)
 
         return data_out
@@ -295,33 +279,25 @@
         db_name=None,
         db_username=None,
         db_password=None,
     ):
         """Initialize DB engine."""
         # Load settings from environment variables
         engine = (
-            db_engine
-            if db_engine is not None
-            else os.environ.get("PYDTK_META_DB_ENGINE", None)
+            db_engine if db_engine is not None else os.environ.get("PYDTK_META_DB_ENGINE", None)
         )
         username = (
             db_username
             if db_username is not None
             else os.environ.get("PYDTK_META_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_META_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_META_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_META_DB_HOST", None)
         database = (
-            db_name
-            if db_name is not None
-            else os.environ.get("PYDTK_META_DB_DATABASE", None)
+            db_name if db_name is not None else os.environ.get("PYDTK_META_DB_DATABASE", None)
         )
 
         super()._initialize_engine(engine, host, database, username, password)
```

### Comparing `pydtk-0.2.9/pydtk/db/v3/handlers/statistics.py` & `pydtk-0.3.0/pydtk/db/v3/handlers/statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,37 +52,29 @@
             else os.environ.get("PYDTK_STATISTICS_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_STATISTICS_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_STATISTICS_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_STATISTICS_DB_HOST", None)
         database = (
-            db_name
-            if db_name is not None
-            else os.environ.get("PYDTK_STATISTICS_DB_DATABASE", None)
+            db_name if db_name is not None else os.environ.get("PYDTK_STATISTICS_DB_DATABASE", None)
         )
 
         super()._initialize_engine(engine, host, database, username, password)
 
     @property
     def _df_name(self):
         """Return _df_name."""
         template = self._config.statistics_df.df_name
         database_id_hashed = hashlib.blake2s(
             self._database_id.encode("utf-8"), digest_size=self._config.hash.digest_size
         ).hexdigest()
-        return template.format(
-            **{"database_id": database_id_hashed, "span": self._span}
-        )
+        return template.format(**{"database_id": database_id_hashed, "span": self._span})
 
     @_df_name.setter
     def _df_name(self, value):
         """Setter for self._df_name."""
         raise RuntimeError("Setting df_name is not supported in StatisticsDBHandler")
 
 
@@ -128,35 +120,27 @@
             else os.environ.get("PYDTK_STATISTICS_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_STATISTICS_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_STATISTICS_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_STATISTICS_DB_HOST", None)
         database = (
-            db_name
-            if db_name is not None
-            else os.environ.get("PYDTK_STATISTICS_DB_DATABASE", None)
+            db_name if db_name is not None else os.environ.get("PYDTK_STATISTICS_DB_DATABASE", None)
         )
 
         super()._initialize_engine(engine, host, database, username, password)
 
     @property
     def _df_name(self):
         """Return _df_name."""
         template = self._config[self._df_class]["df_name"]
         database_id_hashed = hashlib.blake2s(
             self._database_id.encode("utf-8"), digest_size=self._config.hash.digest_size
         ).hexdigest()
-        return template.format(
-            **{"database_id": database_id_hashed, "span": self._span}
-        )
+        return template.format(**{"database_id": database_id_hashed, "span": self._span})
 
     @_df_name.setter
     def _df_name(self, value):
         """Setter for self._df_name."""
         raise RuntimeError("Setting df_name is not supported in StatisticsDBHandler")
```

### Comparing `pydtk-0.2.9/pydtk/db/v3/handlers/time_series.py` & `pydtk-0.3.0/pydtk/db/v3/handlers/time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,15 @@
             else os.environ.get("PYDTK_TIME_SERIES_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_TIME_SERIES_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_TIME_SERIES_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_TIME_SERIES_DB_HOST", None)
         database = (
             db_name
             if db_name is not None
             else os.environ.get("PYDTK_TIME_SERIES_DB_DATABASE", None)
         )
 
         super()._initialize_engine(engine, host, database, username, password)
@@ -159,19 +155,15 @@
             else os.environ.get("PYDTK_TIME_SERIES_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_TIME_SERIES_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_TIME_SERIES_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_TIME_SERIES_DB_HOST", None)
         database = (
             db_name
             if db_name is not None
             else os.environ.get("PYDTK_TIME_SERIES_DB_DATABASE", None)
         )
 
         # Load default settings from config file
@@ -264,17 +256,15 @@
         # Read table from DB
         try:
             res = self._session.execute(str(q), timeout=None)
             df = res._current_rows
         except Exception as e:
             df = self._initialize_df()
             self.logger.warning(
-                'Could not execute SQL statement: "{0}" (reason: {1})'.format(
-                    str(q), str(e)
-                )
+                'Could not execute SQL statement: "{0}" (reason: {1})'.format(str(q), str(e))
             )
 
         self.df = df
 
     def save(self, df=None, **kwargs):
         """Save data to SQL.
 
@@ -289,20 +279,16 @@
 
         # Get column types
         primary_key = ["timestamp"]
         if "record_id" in [c["name"] for c in self.columns]:
             primary_key = ["record_id"] + primary_key
         column_types = cql_df._infer_data_type_from_dtype(primary_key)
         for value in column_types.values():
-            value.column_type = (
-                "double" if value.column_type == "float" else value.column_type
-            )
-            value.column_type = (
-                "double" if value.column_type == "int" else value.column_type
-            )
+            value.column_type = "double" if value.column_type == "float" else value.column_type
+            value.column_type = "double" if value.column_type == "int" else value.column_type
             value.name = '"{}"'.format(value.name)
 
         # Prepare columns
         self._prepare_columns(column_types)
 
         # Write to DB
         cql_df.to_cassandra(
@@ -359,11 +345,10 @@
         return value
 
     @df_name.setter
     def df_name(self, value):
         """Setter for self.df_name."""
         if not re.fullmatch("[a-zA-Z_0-9]+", value):
             raise ValueError(
-                "Invalid df name: {}  "
-                "df name can only contain alphabet, number and underscore"
+                "Invalid df name: {}  " "df name can only contain alphabet, number and underscore"
             )
         self._df_name = value
```

### Comparing `pydtk-0.2.9/pydtk/db/v3/search_engines/__init__.py` & `pydtk-0.3.0/pydtk/db/v3/search_engines/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         if not os.path.isfile(os.path.join(os.path.dirname(__file__), filename)):
             continue
         if filename == "__init__.py":
             continue
 
         try:
             importlib.import_module(
-                os.path.join(
-                    "pydtk.db.v3.search_engines", os.path.splitext(filename)[0]
-                ).replace(os.sep, ".")
+                os.path.join("pydtk.db.v3.search_engines", os.path.splitext(filename)[0]).replace(
+                    os.sep, "."
+                )
             )
         except ModuleNotFoundError:
             logging.debug("Failed to load handlers in {}".format(filename))
 
 
 def register_engine(db_handlers: [T]):
     """Register a DB-search-engine.
```

### Comparing `pydtk-0.2.9/pydtk/db/v3/search_engines/time_series.py` & `pydtk-0.3.0/pydtk/db/v3/search_engines/time_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 from .. import StatisticsCassandraDBHandler as _StatisticsCassandraDBHandler
 from .. import TimeSeriesCassandraDBHandler as _TimeSeriesCassandraDBHandler
 from . import BaseDBSearchEngine as _BaseDBSearchEngine
 from . import register_engine
 
 
-@register_engine(
-    db_handlers=[_TimeSeriesCassandraDBHandler, _StatisticsCassandraDBHandler]
-)
+@register_engine(db_handlers=[_TimeSeriesCassandraDBHandler, _StatisticsCassandraDBHandler])
 class TimeSeriesCassandraDBSearchEngine(_BaseDBSearchEngine):
     """Search engine for V3TimeSeriesCassandraDB."""
 
     def __init__(self, db_handler: _TimeSeriesCassandraDBHandler):
         """Initialize TimeSeriesCassandraDBSearchEngine.
 
         Args:
@@ -44,16 +42,15 @@
             if "like" in condition.lower():
                 raise ValueError(
                     'record_id must be filtered using operator "=" '
                     "(e.g. record_id = '242_16000000080000000570' )"
                 )
             if "'" not in condition:
                 raise ValueError(
-                    "string must be single-quoted "
-                    "(e.g. record_id = '242_16000000080000000570' )"
+                    "string must be single-quoted " "(e.g. record_id = '242_16000000080000000570' )"
                 )
         else:
             if '"' not in condition:
                 raise ValueError(
                     "column name must be double-quoted "
                     '(e.g. "/vehicle/acceleration/accel_linear_x/mean" > 0)'
                 )
```

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/LICENSE` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/LICENSE`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/README.md` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/README.md`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/aggregation_tests.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/aggregation_tests.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/find_tests.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/find_tests.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/__init__.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/aggregation.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/pql/aggregation.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/matching.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/pql/matching.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/setup.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python37/setup.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/LICENSE` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/LICENSE`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/README.md` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/README.md`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/aggregation_tests.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/aggregation_tests.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/find_tests.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/find_tests.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/__init__.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/aggregation.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/pql/aggregation.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/matching.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/pql/matching.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/setup.py` & `pydtk-0.3.0/pydtk/db/v4/deps/pql_python38/setup.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/engines/__init__.py` & `pydtk-0.3.0/pydtk/db/v4/engines/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,14 @@
         if not os.path.isfile(os.path.join(os.path.dirname(__file__), filename)):
             continue
         if filename == "__init__.py":
             continue
 
         try:
             engine_name = str(os.path.splitext(filename)[0])
-            module_name = os.path.join("pydtk.db.v4.engines", engine_name).replace(
-                os.sep, "."
-            )
+            module_name = os.path.join("pydtk.db.v4.engines", engine_name).replace(os.sep, ".")
             DB_ENGINES[engine_name] = importlib.import_module(module_name)
         except ModuleNotFoundError:
             logger.warning("Failed to load DB-engine {}".format(filename))
 
 
 register_engines()
```

### Comparing `pydtk-0.2.9/pydtk/db/v4/engines/mongodb.py` & `pydtk-0.3.0/pydtk/db/v4/engines/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,15 @@
         aggregate = []
         if query:
             aggregate.append({"$match": query})
 
         columns = {}
         for column in set(handler.columns).union(["_uuid", "_creation_time"]):
             try:
-                config = next(
-                    filter(lambda c: c["name"] == column, handler.config["columns"])
-                )
+                config = next(filter(lambda c: c["name"] == column, handler.config["columns"]))
                 agg = config["aggregation"]
                 columns.update({column: {"${}".format(agg): "${}".format(column)}})
             except Exception:
                 columns.update({column: {"$first": "${}".format(column)}})
 
         aggregate.append(
             {
@@ -155,17 +153,15 @@
             aggregate.append({"$skip": offset})
         if limit > 0:
             aggregate.append({"$limit": limit})
 
         data = db.aggregate(aggregate, allowDiskUse=True)
         try:
             count_total = (
-                list(db.aggregate(aggregate_count))[0]["count"]
-                if not disable_count_total
-                else None
+                list(db.aggregate(aggregate_count))[0]["count"] if not disable_count_total else None
             )
         except Exception as e:
             logger.warning(e)
             count_total = None
 
     data = list(data)
     count_total = count_total if count_total is not None else len(data)
```

### Comparing `pydtk-0.2.9/pydtk/db/v4/engines/montydb.py` & `pydtk-0.3.0/pydtk/db/v4/engines/montydb.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,15 @@
 from ..deps import pql as PQL
 
 DEFAULT_DB_NAME = "default"
 DEFAULT_COLLECTION_NAME = "default"
 
 
 def connect(
-    db_host: str,
-    db_name: Optional[str] = None,
-    collection_name: Optional[str] = None,
-    **kwargs
+    db_host: str, db_name: Optional[str] = None, collection_name: Optional[str] = None, **kwargs
 ):
     """Connect to DB.
 
     Args:
         db_host (str): database host
         db_name (str): database name
         collection_name (str): collection name
```

### Comparing `pydtk-0.2.9/pydtk/db/v4/engines/tinydb.py` & `pydtk-0.3.0/pydtk/db/v4/engines/tinydb.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/db/v4/engines/tinymongo.py` & `pydtk-0.3.0/pydtk/db/v4/engines/tinymongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,15 @@
 
     def _new_document(self, key, val):
         doc_id = int(key)
         return Document(val, doc_id)
 
 
 def connect(
-    db_host: str,
-    db_name: Optional[str] = None,
-    collection_name: Optional[str] = None,
-    **kwargs
+    db_host: str, db_name: Optional[str] = None, collection_name: Optional[str] = None, **kwargs
 ):
     """Connect to DB.
 
     Args:
         db_host (str): database host
         db_name (str): database name
         collection_name (str): collection name
@@ -92,19 +89,15 @@
     collection._db_name = db_name
     collection._collection_name = collection_name
 
     return collection
 
 
 def read(
-    db,
-    query: Optional[dict] = None,
-    pql: any = None,
-    order_by: Optional[list] = None,
-    **kwargs
+    db, query: Optional[dict] = None, pql: any = None, order_by: Optional[list] = None, **kwargs
 ):
     """Read data from DB.
 
     Args:
         db (TinyMongoCollection): DB connection
         query (dict or Query): Query to select items
         pql (PQL) Python-Query-Language to select items
```

### Comparing `pydtk-0.2.9/pydtk/db/v4/handlers/__init__.py` & `pydtk-0.3.0/pydtk/db/v4/handlers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import inspect
 import logging
 import os
 from collections.abc import MutableMapping
 from copy import deepcopy
 from datetime import datetime
 
+import iso8601
 import pandas as pd
 from addict import Dict as AttrDict
 from deepmerge import Merger
 
 from pydtk.db.exceptions import DatabaseNotInitializedError, InvalidDatabaseConfigError
 from pydtk.db.schemas import get_schema
 from pydtk.db.v4.engines import DB_ENGINES
@@ -38,17 +39,17 @@
         if not os.path.isfile(os.path.join(os.path.dirname(__file__), filename)):
             continue
         if filename == "__init__.py":
             continue
 
         try:
             importlib.import_module(
-                os.path.join(
-                    "pydtk.db.v4.handlers", str(os.path.splitext(filename)[0])
-                ).replace(os.sep, ".")
+                os.path.join("pydtk.db.v4.handlers", str(os.path.splitext(filename)[0])).replace(
+                    os.sep, "."
+                )
             )
         except ModuleNotFoundError:
             logger.warning("Failed to load handlers in {}".format(filename))
 
 
 def register_handler(db_classes, db_engines):
     """Register a DB-handler.
@@ -89,31 +90,29 @@
     def _fix_dtype(_data, column_conf):
         if column_conf["dtype"].lower() in ["string", "str"]:
             return str(_data)
         elif column_conf["dtype"].lower() in ["integer", "int"]:
             return int(_data)
         elif column_conf["dtype"].lower() in ["float", "double", "number"]:
             return float(_data)
-        elif column_conf["dtype"].lower() in ["list"] or column_conf["dtype"].endswith(
-            "[]"
-        ):
+        elif column_conf["dtype"].lower() in ["list"] or column_conf["dtype"].endswith("[]"):
             return list(_data)
         elif column_conf["dtype"].lower() in ["dict"]:
             return dict(_data)
         elif column_conf["dtype"].lower() in ["datetime"]:
             if isinstance(_data, str):
                 if ":" in _data or "-" in _data:
                     # ISO format
-                    return datetime.fromisoformat(_data)
+                    return iso8601.parse_date(_data)
                 else:
                     raise ValueError(
                         f'Unknown format of datetime: "{_data}"'
                         f"Please make sure to use ISO format (YYYY-mm-dd HH:MM:SS.ffffff)"
                     )
-            elif isinstance(_data, float):
+            elif isinstance(_data, float) or isinstance(_data, int):
                 # Epoch time
                 return datetime.fromtimestamp(_data)
             elif isinstance(_data, datetime):
                 return _data
             else:
                 raise TypeError(
                     f'Unsupported type ({type(_data).__name__}): "{_data}"'
@@ -197,17 +196,15 @@
 
         # Check if the db_class is available
         if db_class not in DB_HANDLERS.keys():
             raise ValueError("Unsupported db_class: {}".format(db_class))
 
         # Get db_engine from environment variable if not specified
         if db_engine is None:
-            db_engine = os.environ.get(
-                "PYDTK_{}_DB_ENGINE".format(db_class.upper()), None
-            )
+            db_engine = os.environ.get("PYDTK_{}_DB_ENGINE".format(db_class.upper()), None)
 
         # Get the default engine if not specified
         if db_engine is None:
             try:
                 db_defaults = getattr(config.db.connection, db_class)
                 db_engine = db_defaults.engine
             except (ValueError, AttributeError):
@@ -398,34 +395,30 @@
         """Save configs to DB."""
         if self._db_engine not in DB_ENGINES.keys():
             return
         try:
             config = dict(self._config)
             config.update({"_uuid": "__config__"})
             config = [config]
-            DB_ENGINES[self._db_engine].upsert(
-                self._config_db, data=config, handler=self
-            )
+            DB_ENGINES[self._db_engine].upsert(self._config_db, data=config, handler=self)
         except Exception as e:
             self.logger.warning("Failed to save configs to DB: {}".format(str(e)))
 
     def _get_uuid_from_item(self, data_in):
         """Return UUID of the given item.
 
         Args:
             data_in (dict or pandas.Series): dict or Series containing data
 
         Returns:
             (str): UUID
 
         """
         hash_target_columns = (
-            self._config["index_columns"]
-            if "index_columns" in self._config.keys()
-            else []
+            self._config["index_columns"] if "index_columns" in self._config.keys() else []
         )
 
         item = data_in
         if isinstance(item, pd.Series):
             item = data_in.to_dict()
 
         pre_hash = "".join(
@@ -445,17 +438,17 @@
 
     def _read(self, **kwargs):
         if self._db_engine is None:
             raise DatabaseNotInitializedError()
         elif self._db_engine in DB_ENGINES.keys():
             func = DB_ENGINES[self._db_engine].read
             available_args = set(inspect.signature(func).parameters.keys())
-            unavailable_args = set(
-                [k for k, v in kwargs.items() if v is not None]
-            ).difference(available_args)
+            unavailable_args = set([k for k, v in kwargs.items() if v is not None]).difference(
+                available_args
+            )
             if len(unavailable_args) > 0:
                 self.logger.warning(
                     'DB-engine "{0}" does not support args: {1}'.format(
                         self._db_engine, list(unavailable_args)
                     )
                 )
             return func(self._db, handler=self, **kwargs)
@@ -528,17 +521,15 @@
             "offset": offset,
             **kwargs,
         }
 
         # Fix data-type
         columns = self._config["columns"] if "columns" in self._config.keys() else []
         for i in range(len(data)):
-            _fix_data_type(
-                data[i], columns, inplace=True, aggregated=group_by is not None
-            )
+            _fix_data_type(data[i], columns, inplace=True, aggregated=group_by is not None)
 
         self._data = {record["_uuid"]: record for record in data}
         self._uuids_duplicated = []
 
     def _upsert(self, data):
         """Upsert data to DB.
 
@@ -601,24 +592,20 @@
         # Remove from DB on saving
         self._tables_to_drop.append(name)
 
         # Remove the corresponding config if exist
         if self._db_engine is None:
             raise DatabaseNotInitializedError()
         elif self._db_engine in DB_ENGINES.keys():
-            if DB_ENGINES[self._db_engine].exist_table(
-                self._db, "--config--{}".format(name)
-            ):
+            if DB_ENGINES[self._db_engine].exist_table(self._db, "--config--{}".format(name)):
                 self._tables_to_drop.append("--config--{}".format(name))
         else:
             raise ValueError("Unsupported DB engine: {}".format(self._db_engine))
 
-    def add_data(
-        self, data_in: dict, strategy="overwrite", ignore_dtype_mismatch=False, **kwargs
-    ):
+    def add_data(self, data_in: dict, strategy="overwrite", ignore_dtype_mismatch=False, **kwargs):
         """Add data to DB-handler.
 
         Args:
             data_in (dict): a dict containing data
             strategy (str): 'merge' or 'overwrite'
             ignore_dtype_mismatch (bool): if True, data type will not be modified
                                           regardless of column specifications
@@ -638,17 +625,15 @@
                 data = self._merger.merge(base_data, data)
             self._uuids_duplicated += [data["_uuid"]]
 
         # Validate data.
         if "_api_version" in data.keys() and "_kind" in data.keys():
             get_schema(data["_api_version"], data["_kind"]).validate(data)
         else:
-            self.logger.warning(
-                "`_api_version` or `_kind` are not defined. Validation is skipped."
-            )
+            self.logger.warning("`_api_version` or `_kind` are not defined. Validation is skipped.")
 
         # Add new columns (keys) to config
         columns = self._config["columns"] if "columns" in self._config.keys() else []
         columns_existing = [c["name"] for c in columns]
         columns_in_data = list(data_in.keys())
         new_columns = []
         for new_column in set(columns_in_data).difference(columns_existing):
@@ -701,34 +686,29 @@
         Returns:
             (pd.DataFrame): a data-frame
 
         """
         columns = self._config["columns"] if "columns" in self._config.keys() else []
         df = pd.concat(
             [
-                pd.Series(
-                    name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"])
-                )
+                pd.Series(name=c["name"], dtype=dtype_string_to_dtype_object(c["dtype"]))
                 for c in columns
                 if c["name"] != "_uuid" and c["name"] != "_creation_time"
             ]  # noqa: E501
             + [
                 pd.Series(name="_uuid", dtype=str),
                 pd.Series(name="_creation_time", dtype=float),
             ],
             axis=1,
         )
         df.set_index("_uuid", inplace=True)
         df = pd.concat([df, pd.DataFrame.from_records(dicts)])
 
         # Apply offset to index
-        if (
-            "offset" in self._read_conditions.keys()
-            and self._read_conditions["offset"] is not None
-        ):
+        if "offset" in self._read_conditions.keys() and self._read_conditions["offset"] is not None:
             df.index += self._read_conditions["offset"]
 
         return df
 
     def _to_display_names(self, df, inplace=False):
         """Rename columns to display-names.
```

### Comparing `pydtk-0.2.9/pydtk/db/v4/handlers/annotation.py` & `pydtk-0.3.0/pydtk/db/v4/handlers/annotation.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 @register_handler(
     db_classes=["annotation"], db_engines=["tinydb", "tinymongo", "mongodb", "montydb"]
 )
 class AnnotationDBHandler(_BaseDBHandler):
     """Handler for annotations."""
 
     __version__ = "v4"
-    db_defaults = load_config(__version__).db.connection.annotations
+    db_defaults = load_config(__version__).db.connection.annotation
     _df_class = "annotation_df"
     _database_id: str = ""
 
     def __init__(self, database_id: str = "default", **kwargs):
         """Initialize AnnotationDBHandler.
 
         Args:
@@ -54,23 +54,17 @@
             else os.environ.get("PYDTK_ANNOTATION_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_ANNOTATION_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_ANNOTATION_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_ANNOTATION_DB_HOST", None)
         database = (
-            db_name
-            if db_name is not None
-            else os.environ.get("PYDTK_ANNOTATION_DB_DATABASE", None)
+            db_name if db_name is not None else os.environ.get("PYDTK_ANNOTATION_DB_DATABASE", None)
         )
 
         super()._initialize_engine(engine, host, database, username, password)
 
     def add_data(self, *args, **kwargs):
         """Add data."""
         super().add_data(*args, **kwargs)
@@ -85,22 +79,18 @@
         """Return _df_name.
 
         Returns:
             (str): name
 
         """
         template = (
-            self._config["_df_name"]
-            if "_df_name" in self._config.keys()
-            else "{database_id}"
+            self._config["_df_name"] if "_df_name" in self._config.keys() else "{database_id}"
         )
         digest_size = (
-            self._config["_hash_digest_size"]
-            if "_hash_digest_size" in self._config.keys()
-            else 4
+            self._config["_hash_digest_size"] if "_hash_digest_size" in self._config.keys() else 4
         )
         database_id_hashed = hashlib.blake2s(
             self._database_id.encode("utf-8"), digest_size=digest_size
         ).hexdigest()
         return template.format(**{"database_id": database_id_hashed})
 
     @_df_name.setter
```

### Comparing `pydtk-0.2.9/pydtk/db/v4/handlers/meta.py` & `pydtk-0.3.0/pydtk/db/v4/handlers/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 from flatten_dict import flatten
 from tqdm import tqdm
 
 from . import BaseDBHandler as _BaseDBHandler
 from . import register_handler
 
 
-@register_handler(
-    db_classes=["meta"], db_engines=["tinydb", "tinymongo", "mongodb", "montydb"]
-)
+@register_handler(db_classes=["meta"], db_engines=["tinydb", "tinymongo", "mongodb", "montydb"])
 class MetaDBHandler(_BaseDBHandler):
     """Handler for metadb."""
 
     _database_id: str = ""
     _df_class = "meta_df"
 
     def __init__(
@@ -47,17 +45,15 @@
         # Solve base-dir
         base_dir = base_dir_path
         if base_dir is None:
             base_dir = "/"
         self.base_dir_path = os.path.realpath(base_dir)
 
         # Prepare another DB-handler for storing a list of database_id
-        self._database_id_db_handler = DatabaseIDDBHandler(
-            **{**kwargs, "read_on_init": False}
-        )
+        self._database_id_db_handler = DatabaseIDDBHandler(**{**kwargs, "read_on_init": False})
 
         # Prepare buffer for iteration
         self._buf = []
         self._indices = []  # [[record_idx, orient_idx]]
         self._indexed = False
 
         super(MetaDBHandler, self).__init__(**kwargs)
@@ -69,52 +65,42 @@
         db_name: Optional[str] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
     ):
         """Initialize DB engine."""
         # Load settings from environment variables
         engine = (
-            db_engine
-            if db_engine is not None
-            else os.environ.get("PYDTK_META_DB_ENGINE", None)
+            db_engine if db_engine is not None else os.environ.get("PYDTK_META_DB_ENGINE", None)
         )
         username = (
             db_username
             if db_username is not None
             else os.environ.get("PYDTK_META_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_META_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_META_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_META_DB_HOST", None)
         database = (
-            db_name
-            if db_name is not None
-            else os.environ.get("PYDTK_META_DB_DATABASE", None)
+            db_name if db_name is not None else os.environ.get("PYDTK_META_DB_DATABASE", None)
         )
 
         super()._initialize_engine(engine, host, database, username, password)
 
     def _solve_path(self, path: str, target: str):
         if target == "relative":
             # noinspection PyTypeChecker
             data_path = Path(path)
             try:
                 relative_path = data_path.relative_to(self.base_dir_path)
                 path = str(relative_path)
             except ValueError as e:
-                logging.warning(
-                    "Could not resolve relative path to file: {}".format(data_path)
-                )
+                logging.warning("Could not resolve relative path to file: {}".format(data_path))
                 logging.warning(str(e))
         elif target == "absolute":
             path = os.path.join(self.base_dir_path, path)
         else:
             raise ValueError("Unrecognized target: {}".format(target))
 
         return path
@@ -137,32 +123,28 @@
 
         # Convert absolute path to relative path
         if "path" in data.keys():
             if isinstance(data["path"], str):
                 data["path"] = self._solve_path(data["path"], target=target)
             elif isinstance(data["path"], list):
                 for idx in range(len(data["path"])):
-                    data["path"][idx] = self._solve_path(
-                        data["path"][idx], target=target
-                    )
+                    data["path"][idx] = self._solve_path(data["path"][idx], target=target)
             else:
                 raise TypeError("Unsupported type")
 
         return data
 
     def _reindex(self):
         """Re-index."""
         indices = []
 
         for idx, value in enumerate(self._data.values()):
             # Count for self.__len__
             if self.orient in value.keys():
-                if isinstance(value[self.orient], dict) or isinstance(
-                    value[self.orient], list
-                ):
+                if isinstance(value[self.orient], dict) or isinstance(value[self.orient], list):
                     indices += [[idx, i] for i in range(len(value[self.orient]))]
                 else:
                     indices += [[idx, 0]]
             else:
                 indices += [[idx, 0]]
 
         self._indices = indices
@@ -201,17 +183,17 @@
         data = self._solve_path_in_data(data, target="absolute")
 
         data = deepcopy(data)
 
         if self.orient in data.keys():
             if isinstance(data[self.orient], dict):
                 data[self.orient] = {
-                    list(data[self.orient].keys())[orient_idx]: list(
-                        data[self.orient].values()
-                    )[orient_idx]
+                    list(data[self.orient].keys())[orient_idx]: list(data[self.orient].values())[
+                        orient_idx
+                    ]
                 }
             if isinstance(data[self.orient], list):
                 data[self.orient] = [data[self.orient][orient_idx]]
 
         return data
 
     def add_data(self, data_in: dict, **kwargs):
@@ -301,27 +283,21 @@
             data (dict): a dict to update as type file.
 
         Returns:
             (dict): data updated as type file.
 
         """
         data["_kind"] = "file"
-        assert (
-            "path" in data.keys()
-        ), "The 'file' type data must have 'path' information."
+        assert "path" in data.keys(), "The 'file' type data must have 'path' information."
 
         # Get uuid of parent's metadata
         hash_target_columns = (
-            self._config["index_columns"]
-            if "index_columns" in self._config.keys()
-            else []
-        )
-        parent_data = {
-            key: value for key, value in data.items() if key in hash_target_columns
-        }
+            self._config["index_columns"] if "index_columns" in self._config.keys() else []
+        )
+        parent_data = {key: value for key, value in data.items() if key in hash_target_columns}
         parent_data.update({"_kind": "record", "path": ""})
         data["_record"] = self._get_uuid_from_item(parent_data)
 
         return data
 
     def read(self, *args, **kwargs):
         """Read function."""
@@ -387,18 +363,15 @@
     def data(self):
         """Return data.
 
         Returns:
             (list): list of dicts
 
         """
-        return [
-            self._solve_path_in_data(data, target="absolute")
-            for data in self._data.values()
-        ]
+        return [self._solve_path_in_data(data, target="absolute") for data in self._data.values()]
 
     @data.setter
     def data(self, data):
         """Setter for self.data.
 
         Args:
             data (list): new-data
@@ -418,22 +391,18 @@
         """Return _df_name.
 
         Returns:
             (str): name
 
         """
         template = (
-            self._config["_df_name"]
-            if "_df_name" in self._config.keys()
-            else "{database_id}"
+            self._config["_df_name"] if "_df_name" in self._config.keys() else "{database_id}"
         )
         digest_size = (
-            self._config["_hash_digest_size"]
-            if "_hash_digest_size" in self._config.keys()
-            else 4
+            self._config["_hash_digest_size"] if "_hash_digest_size" in self._config.keys() else 4
         )
         database_id_hashed = hashlib.blake2s(
             self._database_id.encode("utf-8"), digest_size=digest_size
         ).hexdigest()
         return template.format(**{"database_id": database_id_hashed})
 
     @_df_name.setter
@@ -457,17 +426,15 @@
                         value = flatten(next(iter(_data[self.orient])), reducer="dot")
                         _data = self._merger.merge(_data, value)
                     else:
                         _data[self.orient] = _data[self.orient][0]
                 elif isinstance(_data[self.orient], dict):
                     assert len(_data[self.orient]) == 1
                     key = next(iter(_data[self.orient].keys()))
-                    value = flatten(
-                        next(iter(_data[self.orient].values())), reducer="dot"
-                    )
+                    value = flatten(next(iter(_data[self.orient].values())), reducer="dot")
                     _data[self.orient] = key
                     _data = self._merger.merge(_data, value)
                 else:
                     pass
             data.append(_data)
 
         df = self._df_from_dicts(data)
@@ -497,37 +464,29 @@
         db_name: Optional[str] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
     ):
         """Initialize DB engine."""
         # Load settings from environment variables
         engine = (
-            db_engine
-            if db_engine is not None
-            else os.environ.get("PYDTK_META_DB_ENGINE", None)
+            db_engine if db_engine is not None else os.environ.get("PYDTK_META_DB_ENGINE", None)
         )
         username = (
             db_username
             if db_username is not None
             else os.environ.get("PYDTK_META_DB_USERNAME", None)
         )
         password = (
             db_password
             if db_password is not None
             else os.environ.get("PYDTK_META_DB_PASSWORD", None)
         )
-        host = (
-            db_host
-            if db_host is not None
-            else os.environ.get("PYDTK_META_DB_HOST", None)
-        )
+        host = db_host if db_host is not None else os.environ.get("PYDTK_META_DB_HOST", None)
         database = (
-            db_name
-            if db_name is not None
-            else os.environ.get("PYDTK_META_DB_DATABASE", None)
+            db_name if db_name is not None else os.environ.get("PYDTK_META_DB_DATABASE", None)
         )
 
         super()._initialize_engine(engine, host, database, username, password)
 
     def remove_data(self, data, cascade=True):
         """Remove data from DB.
```

### Comparing `pydtk-0.2.9/pydtk/frontend.py` & `pydtk-0.3.0/pydtk/frontend.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/io/reader.py` & `pydtk-0.3.0/pydtk/io/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,22 +49,15 @@
     def model(self, model):
         self._model = model
 
     def add_preprocess(self, preprocess):
         """Add preprocessing function."""
         self.preprocesses += [preprocess]
 
-    def read(
-        self,
-        metadata=None,
-        as_generator=False,
-        model_kwargs=None,
-        as_ndarray=True,
-        **kwargs
-    ):
+    def read(self, metadata=None, as_generator=False, model_kwargs=None, as_ndarray=True, **kwargs):
         """Read a file which corresponds to the given metadata.
 
         Args:
             metadata (MetaDataModel or dict): metadata of the data to load
             as_generator (bool): load data as a generator.
             model_kwargs (dict): kwargs to pass to the selected model
 
@@ -91,25 +84,21 @@
                     metadata.load(metadata_filepath)
             if metadata is None:
                 raise IOError("Could not find metadata file")
         else:
             metadata = MetaDataModel(metadata)
 
         # Replace 'contents' in metadata to specify which content to load
-        contents = (
-            metadata.data["contents"] if "contents" in metadata.data.keys() else None
-        )
+        contents = metadata.data["contents"] if "contents" in metadata.data.keys() else None
         if "contents" in kwargs.keys():
             if isinstance(kwargs["contents"], dict):
                 contents = kwargs["contents"]
             if isinstance(kwargs["contents"], str):
                 contents = next(
-                    iter(
-                        [{k: v for k, v in contents.items() if k == kwargs["contents"]}]
-                    )
+                    iter([{k: v for k, v in contents.items() if k == kwargs["contents"]}])
                 )
             if len(contents) == 0:
                 raise ValueError("No corresponding contents exist")
 
         # Replace other attributes with the given arguments
         metadata.data.update(kwargs)
         metadata.data.update({"contents": contents})
```

### Comparing `pydtk-0.2.9/pydtk/io/writer.py` & `pydtk-0.3.0/pydtk/io/writer.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/models/__init__.py` & `pydtk-0.3.0/pydtk/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,15 @@
     """Register models."""
     for filename in os.listdir(os.path.join(os.path.dirname(__file__))):
         if filename == "__init__.py":
             continue
 
         try:
             importlib.import_module(
-                os.path.join("pydtk.models", os.path.splitext(filename)[0]).replace(
-                    os.sep, "."
-                )
+                os.path.join("pydtk.models", os.path.splitext(filename)[0]).replace(os.sep, ".")
             )
         except (ModuleNotFoundError, ImportError):
             logger.warning("Failed to load models in {}".format(filename))
 
 
 def register_model(priority=0):
     """Regist a model."""
@@ -72,17 +70,15 @@
         super(MetaDataModel, self).__init__(**kwargs)
         if data is not None:
             if isinstance(data, MetaDataModel):
                 self.data = data.data
             elif isinstance(data, dict):
                 self.data = data
             else:
-                raise TypeError(
-                    "Unsupported type of data: {}".format(type(data).__name__)
-                )
+                raise TypeError("Unsupported type of data: {}".format(type(data).__name__))
 
     @classmethod
     def is_loadable(cls, path="", **kwargs):
         """Check file format."""
         _, ext = os.path.splitext(path)
         if ext not in cls._file_extensions:
             return False
@@ -204,24 +200,20 @@
         for key, value in kwargs.items():
             if key in self._config.keys():
                 self._config[key] = value
             else:
                 raise KeyError("Unknown key: {}".format(key))
 
     @classmethod
-    def _is_loadable(
-        cls, path="", contents=None, content_type=None, data_type=None, **kwargs
-    ):
+    def _is_loadable(cls, path="", contents=None, content_type=None, data_type=None, **kwargs):
         """Check data by file format."""
         return True
 
     @classmethod
-    def is_loadable(
-        cls, path="", contents=None, content_type=None, data_type=None, **kwargs
-    ):
+    def is_loadable(cls, path="", contents=None, content_type=None, data_type=None, **kwargs):
         """Check if the given file is loadable.
 
         Args:
             path (str): path to the target file
             contents (dict or str): content to load (e.g. {'camera/front': 'tags': {...}})
             content_type (str): content-type (e.g. 'text/csv')
             data_type (str): data-type (e.g. 'raw_data')
@@ -253,20 +245,15 @@
         # check by contents
         if cls._contents is not None:
             if contents is None:
                 if isinstance(cls._contents, str):
                     if re.fullmatch(cls._contents, "") is None:
                         return False
                 if isinstance(cls._contents, list):
-                    if (
-                        any(
-                            [re.fullmatch(_contents, "") for _contents in cls._contents]
-                        )
-                        is False
-                    ):
+                    if any([re.fullmatch(_contents, "") for _contents in cls._contents]) is False:
                         return False
                 if isinstance(cls._contents, dict):
                     if re.fullmatch(next(iter(cls._contents)), "") is None:
                         return False
             else:
                 if isinstance(contents, dict) and len(contents.keys()) > 1:
                     logging.warning("Loading multiple contents is not supported")
@@ -280,20 +267,15 @@
                     if re.fullmatch(cls._contents, contents) is None:
                         return False
                 if isinstance(cls._contents, str) and isinstance(contents, dict):
                     if re.fullmatch(cls._contents, next(iter(contents))) is None:
                         return False
                 if isinstance(cls._contents, list) and isinstance(contents, str):
                     if (
-                        any(
-                            [
-                                re.fullmatch(_contents, contents)
-                                for _contents in cls._contents
-                            ]
-                        )
+                        any([re.fullmatch(_contents, contents) for _contents in cls._contents])
                         is False
                     ):
                         return False
                 if isinstance(cls._contents, list) and isinstance(contents, dict):
                     if (
                         any(
                             [
@@ -309,19 +291,15 @@
                         return False
                 if isinstance(cls._contents, dict) and isinstance(contents, dict):
                     if dict_reg_match(cls._contents, contents) is False:
                         return False
 
         # check data by file format
         if not cls._is_loadable(
-            path=path,
-            contents=contents,
-            content_type=content_type,
-            data_type=data_type,
-            **kwargs
+            path=path, contents=contents, content_type=content_type, data_type=data_type, **kwargs
         ):
             return False
 
         # in case all check passed
         return True
 
     @property
@@ -364,17 +342,15 @@
         """
         assert any([isinstance(metadata, dict), isinstance(metadata, MetaDataModel)])
         if isinstance(metadata, dict):
             metadata = MetaDataModel(data=metadata)
         self._metadata = metadata
 
     @abstractmethod
-    def _load(
-        self, path, contents=None, start_timestamp=None, end_timestamp=None, **kwargs
-    ):
+    def _load(self, path, contents=None, start_timestamp=None, end_timestamp=None, **kwargs):
         """Load data from a file.
 
         Args:
             path (str): path to the input file
             contents (dict or str): content to load
             start_timestamp (float): timestamp to start loading in sec.
             end_timestamp (float): timestamp to end loading in sec.
@@ -408,17 +384,15 @@
 
         # update metadata
         self.metadata = metadata
 
         # check if this model can load the data
         if not self.is_loadable(**metadata.data):
             raise UnsupportedFileError(
-                'Model "{0}" does not support loading file: {1}'.format(
-                    type(self).__name__, path
-                )
+                'Model "{0}" does not support loading file: {1}'.format(type(self).__name__, path)
             )
 
         if as_generator:
 
             def load_as_generator():
                 yield from self._load_as_generator(**metadata.data)
 
@@ -443,17 +417,15 @@
                 raise ValueError("filepath is not provided")
             else:
                 path = self.metadata.data["path"]
 
         # check
         _, ext = os.path.splitext(path)
         if ext.lower() not in self._file_extensions:
-            raise ValueError(
-                "File extension must be one of: {}".format(self._file_extensions)
-            )
+            raise ValueError("File extension must be one of: {}".format(self._file_extensions))
 
         # save
         self._save(path=path, **kwargs)
 
     @property
     def columns(self):
         """Return the name of each column in ndarray returned from `to_ndarray`."""
```

### Comparing `pydtk-0.2.9/pydtk/models/autoware/can_packet.py` & `pydtk-0.3.0/pydtk/models/autoware/can_packet.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,15 @@
         if path_to_assign_list is not None:
             self._config["path_to_assign_list"] = path_to_assign_list
             self.can_decoder = CANDecoder(path_to_assign_list)
 
     def msg_to_data(self, msg, **kwargs):
         """Convert a message to data."""
         if self.can_decoder is not None:
-            can_id = (
-                bitstring.ConstBitArray(uint=int(msg.id), length=32)
-                .hex.lstrip("0")
-                .lower()
-            )
+            can_id = bitstring.ConstBitArray(uint=int(msg.id), length=32).hex.lstrip("0").lower()
             can_data = bitstring.ConstBitArray(bytes=msg.dat).hex
 
             data = []
             for bit_assign in self.can_decoder.bit_assign_info.signal_list.values():
                 if can_id.replace(" ", "") == bit_assign.can_id:
                     data.append(self.can_decoder.unpack_data(can_data, bit_assign))
                 else:
```

### Comparing `pydtk-0.2.9/pydtk/models/csv.py` & `pydtk-0.3.0/pydtk/models/csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,15 @@
         Args:
             path (str): path to a csv file
             start_timestamp (float): timestamp to start loading (not supported)
             end_timestamp (float): timestamp to end loading (not supported)
 
         """
         if start_timestamp is not None and end_timestamp is not None:
-            raise ValueError(
-                "Specifying time-range to load is not supported in GenericCsvModel"
-            )
+            raise ValueError("Specifying time-range to load is not supported in GenericCsvModel")
         data = pd.read_csv(path, header=None).to_numpy()
         self.data = data
 
     def _save(self, path, **kwargs):
         """Save ndarray data to a csv file.
 
         Args:
```

### Comparing `pydtk-0.2.9/pydtk/models/image.py` & `pydtk-0.3.0/pydtk/models/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,15 @@
         """
         # Load file
         data = cv2.imread(path)
         shape = data.shape
         _, ext = os.path.splitext(path)
 
         # Generate metadata
-        contents = {
-            content_key: {"size": shape, "tags": ["image", ext.replace(".", "")]}
-        }
+        contents = {content_key: {"size": shape, "tags": ["image", ext.replace(".", "")]}}
 
         return contents
 
     @property
     def timestamps(self, path):
         """Return timestamps as ndarray."""
         raise NotImplementedError
```

### Comparing `pydtk-0.2.9/pydtk/models/json_model.py` & `pydtk-0.3.0/pydtk/models/json_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,15 @@
         if "time_stamps" in self.data.keys():
             return np.ndarray(self.data["time_stamps"])
 
         return np.ndarray([])
 
     def to_ndarray(self):
         """Json model do not support to_ndarray."""
-        raise AttributeError(
-            "JsonModel do not support to_ndarray, since it may be semi-structured"
-        )
+        raise AttributeError("JsonModel do not support to_ndarray, since it may be semi-structured")
 
     @classmethod
     def generate_contents_meta(cls, path, content_key="content"):
         """Generate contents metadata.
 
         Args:
             path (str): File path
```

### Comparing `pydtk-0.2.9/pydtk/models/movie.py` & `pydtk-0.3.0/pydtk/models/movie.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,15 @@
         else:
             start_frame_idx = 0
         if end_timestamp is not None:
             end_frame_idx = min(np.ceil(end_timestamp * fps).astype(int), n_frames - 1)
         else:
             end_frame_idx = n_frames - 1
         frame_size = end_frame_idx - start_frame_idx + 1
-        assert (
-            0 <= start_frame_idx <= end_frame_idx < n_frames
-        ), "Timestamp out of range!"
+        assert 0 <= start_frame_idx <= end_frame_idx < n_frames, "Timestamp out of range!"
 
         # Read video
         cap.set(cv2.CAP_PROP_POS_FRAMES, start_frame_idx)
         data = np.empty((frame_size, height, width, n_channels), dtype=np.uint8)
         timestamps = [0.0 for _ in range(frame_size)]
         for seek_idx in range(frame_size):
             frame_idx = start_frame_idx + seek_idx
@@ -80,17 +78,15 @@
 
             # Store frames and timestamps
             ret, frame = cap.read()
             if ret:
                 data[seek_idx] = frame
                 timestamps[seek_idx] = sec_current
             else:
-                assert (
-                    frame_idx == end_frame_idx
-                ), "Reading frame unexpectedly finished!"
+                assert frame_idx == end_frame_idx, "Reading frame unexpectedly finished!"
                 break
 
         # Close stream
         cap.release()
 
         self.data = {
             "timestamps": timestamps,
@@ -122,20 +118,20 @@
 
         frames = self.data["data"]
         fmt = cv2.VideoWriter_fourcc(*"mp4v")
         size = (width, height)
         writer = cv2.VideoWriter(path, fmt, fps, size)
 
         for frame in frames:
-            assert (
-                frame.shape[0] == height
-            ), "Resolution mismatched! (height {} != {})".format(height, frame.shape[0])
-            assert (
-                frame.shape[1] == width
-            ), "Resolution mismatched! (width {} != {})".format(width, frame.shape[1])
+            assert frame.shape[0] == height, "Resolution mismatched! (height {} != {})".format(
+                height, frame.shape[0]
+            )
+            assert frame.shape[1] == width, "Resolution mismatched! (width {} != {})".format(
+                width, frame.shape[1]
+            )
             writer.write(frame)
 
         writer.release()
 
     def to_ndarray(self):
         """Return data as ndarray."""
         return np.array(self.data["data"])
@@ -197,17 +193,15 @@
         n_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
 
         # Load the first frame and get information
         ret, frame = cap.read()
         frame_info = {}
         if ret:
             height, width, n_channels = frame.shape
-            frame_info.update(
-                {"height": height, "width": width, "n_channels": n_channels}
-            )
+            frame_info.update({"height": height, "width": width, "n_channels": n_channels})
 
         # Get duration
         cap.set(cv2.CAP_PROP_POS_FRAMES, n_frames)
         duration = cap.get(cv2.CAP_PROP_POS_MSEC) / 1000.0
 
         # Close the file
         cap.release()
@@ -296,17 +290,15 @@
         timestamps_reader = CameraTimestampCsvModel(metadata=timestamps_metadata)
         timestamps_reader._load(timestamps_path)
         timestamps = timestamps_reader.timestamps
 
         cap = cv2.VideoCapture(path)
         n_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         if not raw:
-            timestamps = self.downsample_frames(
-                timestamps, target_frame_rate=target_frame_rate
-            )
+            timestamps = self.downsample_frames(timestamps, target_frame_rate=target_frame_rate)
         assert n_frames == len(timestamps)
 
         frame_indices = np.arange(0, n_frames)
         frame_indices = frame_indices[
             np.logical_and(timestamps >= start_timestamp, timestamps < end_timestamp)
         ]
         timestamps = timestamps[frame_indices]
```

### Comparing `pydtk-0.2.9/pydtk/models/pointcloud/pcd.py` & `pydtk-0.3.0/pydtk/models/pointcloud/pcd.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/models/rosbag.py` & `pydtk-0.3.0/pydtk/models/rosbag.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,15 @@
                 idx = 0
             for topic, msg, t in bag.read_messages(
                 topics=[topic], start_time=start_time, end_time=end_time
             ):
                 timestamp = self.msg_to_timestamp(msg, t).to_sec()
                 if target_frame_rate:
                     if timestamp == timestamps[idx]:
-                        data.append(
-                            self.msg_to_data(msg, config=self._config, **kwargs)
-                        )
+                        data.append(self.msg_to_data(msg, config=self._config, **kwargs))
                         idx += 1
                         if idx == len(timestamps):
                             break
                     continue
                 timestamps.append(timestamp)
                 data.append(self.msg_to_data(msg, config=self._config, **kwargs))
 
@@ -133,17 +131,15 @@
                 topics=[topic], start_time=start_time, end_time=end_time
             ):
                 timestamp = self.msg_to_timestamp(msg, t).to_sec()
                 if target_frame_rate:
                     if timestamp == timestamps[idx]:
                         yield {
                             "timestamps": [timestamp],
-                            "data": [
-                                self.msg_to_data(msg, config=self._config, **kwargs)
-                            ],
+                            "data": [self.msg_to_data(msg, config=self._config, **kwargs)],
                         }
                         idx += 1
                         if idx == len(timestamps):
                             break
                     continue
                 yield {
                     "timestamps": [timestamp],
@@ -331,17 +327,15 @@
     def msg_to_data(self, msg, **kwargs):
         """Convert a message to data."""
         if msg.__class__.__name__ == "_sensor_msgs__PointCloud2":
             msg.__class__ = sensor_msgs.msg._PointCloud2.PointCloud2
         points = ros_numpy.numpify(msg)[list(self._config["fields"])]
         pointcloud = np.array(points.tolist())
         if "intensity" in self._config["fields"]:
-            pointcloud[
-                :, self._config["fields"].index("intensity")
-            ] /= 255.0  # scale to [0, 1]
+            pointcloud[:, self._config["fields"].index("intensity")] /= 255.0  # scale to [0, 1]
         return pointcloud
 
     def to_ndarray(self):
         """Return data as ndarray."""
         return np.array(self.data["data"], dtype="object")
 
     @property
```

### Comparing `pydtk-0.2.9/pydtk/models/rosbag2.py` & `pydtk-0.3.0/pydtk/models/rosbag2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Copyright Toolkit Authors
 
 import glob
 import logging
 import os.path as osp
 import platform
 from abc import ABC
+from importlib.metadata import version as get_version
 
 import numpy as np
 import rosbag2_py
 from packaging import version
 from pandas import DataFrame
 from rclpy.serialization import deserialize_message
 from rosidl_runtime_py.utilities import get_message
@@ -20,14 +21,17 @@
 
 # check python version
 python_version = ".".join(platform.python_version_tuple()[:2])
 if version.parse(python_version) != version.parse("3.10"):
     raise ImportError(
         f"ROS2 (Humble) supports only Python 3.10, but your Python is {python_version}"
     )
+# check rosbag2_py version
+rosbag2_py_version = get_version("rosbag2_py")
+is_mcap_seeking_supported = version.parse(rosbag2_py_version) >= version.parse("0.15.4")
 
 
 def get_rosbag_options(
     path,
     storage_id,
     serialization_format="cdr",
 ):
@@ -89,35 +93,33 @@
         if isinstance(contents, str):
             topic = contents
         if isinstance(contents, dict):
             topic = next(iter(contents))
         if topic is None:
             raise ValueError('Topic name must be specified by the argument "contents"')
 
-        # NOTE(kan-bayashi): Seek with mcap does not work well in 2022/12/27
-        # TODO(kan-bayashi): May next ROS2 support seek with mcap format
-        #   https://github.com/ros2/rosbag2/pull/1205
+        # NOTE: Seek with mcap does not work well with rosbag2_py < v0.15.4.
+        #       https://github.com/ros2/rosbag2/pull/1205
         if start_timestamp is not None and self._get_storage_id(path) == "mcap":
-            self.logger.warning("start_timestamp is not supported. ignored.")
-            start_timestamp = None
+            if not is_mcap_seeking_supported:
+                self.logger.warning("start_timestamp is not supported. ignored.")
+                start_timestamp = None
 
         # Load rosbag2
         reader = rosbag2_py.SequentialReader()
         reader.open(*get_rosbag_options(path, self._get_storage_id(path)))
 
         # Seek timestamp if needed
         if start_timestamp is not None:
             # TODO(kan-bayashi): What happened when start timestamp if exceed end timestamp?
             reader.seek(int(start_timestamp * 10**9))
 
         # Create mapping dict of topic name and type
         topic_types = reader.get_all_topics_and_types()
-        type_map = {
-            topic_types[i].name: topic_types[i].type for i in range(len(topic_types))
-        }
+        type_map = {topic_types[i].name: topic_types[i].type for i in range(len(topic_types))}
         assert topic in type_map, f"topic {topic} is not included in rosbag."
 
         # Set filter
         storage_filter = rosbag2_py.StorageFilter(topics=[topic])
         reader.set_filter(storage_filter)
 
         if target_frame_rate is not None:
@@ -191,35 +193,33 @@
         if isinstance(contents, str):
             topic = contents
         if isinstance(contents, dict):
             topic = next(iter(contents))
         if topic is None:
             raise ValueError('Topic name must be specified by the argument "contents"')
 
-        # NOTE(kan-bayashi): Seek with mcap does not work well in 2022/12/27
-        # TODO(kan-bayashi): May next ROS2 support seek with mcap format
-        #   https://github.com/ros2/rosbag2/pull/1205
+        # NOTE: Seek with mcap does not work well with rosbag2_py < v0.15.4.
+        #       https://github.com/ros2/rosbag2/pull/1205
         if start_timestamp is not None and self._get_storage_id(path) == "mcap":
-            self.logger.warning("start_timestamp is not supported. ignored.")
-            start_timestamp = None
+            if not is_mcap_seeking_supported:
+                self.logger.warning("start_timestamp is not supported. ignored.")
+                start_timestamp = None
 
         # Load rosbag2
         reader = rosbag2_py.SequentialReader()
         reader.open(*get_rosbag_options(path, self._get_storage_id(path)))
 
         # Seek timestamp if needed
         if start_timestamp is not None:
             # TODO(kan-bayashi): What happened when start timestamp if exceed end timestamp?
             reader.seek(int(start_timestamp * 10**9))
 
         # Create mapping dict of topic name and type
         topic_types = reader.get_all_topics_and_types()
-        type_map = {
-            topic_types[i].name: topic_types[i].type for i in range(len(topic_types))
-        }
+        type_map = {topic_types[i].name: topic_types[i].type for i in range(len(topic_types))}
         assert topic in type_map, f"topic {topic} is not included in rosbag."
 
         # Set filter
         storage_filter = rosbag2_py.StorageFilter(topics=[topic])
         reader.set_filter(storage_filter)
 
         if target_frame_rate is not None:
```

### Comparing `pydtk-0.2.9/pydtk/models/zstd/rosbag.py` & `pydtk-0.3.0/pydtk/models/zstd/rosbag.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,17 +130,15 @@
     def msg_to_data(self, msg, **kwargs):
         """Convert a message to data."""
         if msg.__class__.__name__ == "_sensor_msgs__PointCloud2":
             msg.__class__ = sensor_msgs.msg._PointCloud2.PointCloud2
         points = ros_numpy.numpify(msg)[list(self._config["fields"])]
         pointcloud = np.array(points.tolist())
         if "intensity" in self._config["fields"]:
-            pointcloud[
-                :, self._config["fields"].index("intensity")
-            ] /= 255.0  # scale to [0, 1]
+            pointcloud[:, self._config["fields"].index("intensity")] /= 255.0  # scale to [0, 1]
         return pointcloud
 
     def to_ndarray(self):
         """Return data as ndarray."""
         return np.array(self.data["data"], dtype="object")
 
     @property
```

### Comparing `pydtk-0.2.9/pydtk/preprocesses/downsampling.py` & `pydtk-0.3.0/pydtk/preprocesses/downsampling.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/preprocesses/passthrough.py` & `pydtk-0.3.0/pydtk/preprocesses/passthrough.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/statistics/__init__.py` & `pydtk-0.3.0/pydtk/statistics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,15 @@
 
         Returns:
             index_timestamps (ndarray): timestamps [sec]
             stat_data (ndarray): mean of input data
 
         """
         self.calculator = self._get_calculator(str(data.dtype))
-        index_timestamps, stat_data = getattr(self.calculator, operation)(
-            timestamps, data
-        )
+        index_timestamps, stat_data = getattr(self.calculator, operation)(timestamps, data)
         return index_timestamps, stat_data
 
     def mean(self, timestamps, data):
         """Divide and return means of divided data."""
         return self.calculate(timestamps, data, "mean")
 
     def max(self, timestamps, data):
```

### Comparing `pydtk-0.2.9/pydtk/statistics/calculator.py` & `pydtk-0.3.0/pydtk/statistics/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,15 @@
 
         """
         # Initialize the output array and buffers
         divided_timestamps, divided_data = [], []
         buffer_timestamps, buffer_data = [], []
 
         # Calculate the first timestamp-index
-        fps_previous_index = (
-            timestamps[0] // float(self.target_span) if len(timestamps) > 0 else 0
-        )
+        fps_previous_index = timestamps[0] // float(self.target_span) if len(timestamps) > 0 else 0
 
         # Read over the data to store timestamps and data
         for timestamp, value in zip(timestamps, data):
             fps_current_index = timestamp // float(self.target_span)
 
             if fps_current_index == fps_previous_index:
                 # Store data into the buffer in case of the same timestamp-index
@@ -85,41 +83,33 @@
 
         divided_timestamps = np.array(divided_timestamps)
         return divided_timestamps, divided_data
 
     def mean(self, timestamps, data):
         """Divide and return means of divided data."""
         raise UnsupportedOperationError(
-            "Model '{0}' does not support operation: {1}".format(
-                type(self).__name__, "mean"
-            )
+            "Model '{0}' does not support operation: {1}".format(type(self).__name__, "mean")
         )
 
     def max(self, timestamps, data):
         """Divide and return maximum of divided data."""
         raise UnsupportedOperationError(
-            "Model '{0}' does not support operation: {1}".format(
-                type(self).__name__, "max"
-            )
+            "Model '{0}' does not support operation: {1}".format(type(self).__name__, "max")
         )
 
     def min(self, timestamps, data):
         """Divide and return minimum of divided data."""
         raise UnsupportedOperationError(
-            "Model '{0}' does not support operation: {1}".format(
-                type(self).__name__, "min"
-            )
+            "Model '{0}' does not support operation: {1}".format(type(self).__name__, "min")
         )
 
     def count(self, timestamps, data):
         """Divide and return count of True in divided data."""
         raise UnsupportedOperationError(
-            "Model '{0}' does not support operation: {1}".format(
-                type(self).__name__, "count"
-            )
+            "Model '{0}' does not support operation: {1}".format(type(self).__name__, "count")
         )
 
 
 class FloatCalculator(BaseCalculator):
     """Calculator for data of float."""
 
     def __init__(self, target_span=60.0, **kwargs):
@@ -137,16 +127,15 @@
             index_timestamps (ndarray): timestamps [sec]
             stat_data (ndarray): mean of input data
 
         """
         index_timestamps, divided_data = self.divide(timestamps, data)
         data_dim = data.ndim
         stat_data = [
-            values.mean(axis=0) if values.ndim == data_dim else values
-            for values in divided_data
+            values.mean(axis=0) if values.ndim == data_dim else values for values in divided_data
         ]
         stat_data = np.array(stat_data)
         return index_timestamps, stat_data
 
     def max(self, timestamps, data):
         """Calculate max.
 
@@ -158,16 +147,15 @@
             index_timestamps (ndarray): timestamps [sec]
             stat_data (ndarray): max of input data
 
         """
         index_timestamps, divided_data = self.divide(timestamps, data)
         data_dim = data.ndim
         stat_data = [
-            values.max(axis=0) if values.ndim == data_dim else values
-            for values in divided_data
+            values.max(axis=0) if values.ndim == data_dim else values for values in divided_data
         ]
         stat_data = np.array(stat_data)
         return index_timestamps, stat_data
 
     def min(self, timestamps, data):
         """Calculate minimum.
 
@@ -179,16 +167,15 @@
             index_timestamps (ndarray): timestamps [sec]
             stat_data (ndarray): min of input data
 
         """
         index_timestamps, divided_data = self.divide(timestamps, data)
         data_dim = data.ndim
         stat_data = [
-            values.min(axis=0) if values.ndim == data_dim else values
-            for values in divided_data
+            values.min(axis=0) if values.ndim == data_dim else values for values in divided_data
         ]
         stat_data = np.array(stat_data)
         return index_timestamps, stat_data
 
 
 class BoolCalculator(BaseCalculator):
     """Calculator for data of float."""
@@ -208,16 +195,15 @@
             index_timestamps (ndarray): timestamps [sec]
             stat_data (ndarray): count of true data
 
         """
         index_timestamps, divided_data = self.divide(timestamps, data)
         data_dim = data.ndim
         stat_data = [
-            values.sum(axis=0) if values.ndim == data_dim else values
-            for values in divided_data
+            values.sum(axis=0) if values.ndim == data_dim else values for values in divided_data
         ]
         stat_data = np.array(stat_data)
         return index_timestamps, stat_data
 
     def mean(self, timestamps, data):
         """Average of true counts during the span.
 
@@ -243,16 +229,15 @@
             index_timestamps (ndarray): timestamps [sec]
             stat_data (ndarray): max of input data
 
         """
         index_timestamps, divided_data = self.divide(timestamps, data)
         data_dim = data.ndim
         stat_data = [
-            values.max(axis=0) if values.ndim == data_dim else values
-            for values in divided_data
+            values.max(axis=0) if values.ndim == data_dim else values for values in divided_data
         ]
         stat_data = np.array(stat_data)
         return index_timestamps, stat_data
 
     def min(self, timestamps, data):
         """Calculate minimum.
 
@@ -264,12 +249,11 @@
             index_timestamps (ndarray): timestamps [sec]
             stat_data (ndarray): min of input data
 
         """
         index_timestamps, divided_data = self.divide(timestamps, data)
         data_dim = data.ndim
         stat_data = [
-            values.min(axis=0) if values.ndim == data_dim else values
-            for values in divided_data
+            values.min(axis=0) if values.ndim == data_dim else values for values in divided_data
         ]
         stat_data = np.array(stat_data)
         return index_timestamps, stat_data
```

### Comparing `pydtk-0.2.9/pydtk/utils/can_decoder.py` & `pydtk-0.3.0/pydtk/utils/can_decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,17 +128,15 @@
         self.logger.debug(
             "loaded {0} signal assignment from file: {1}".format(
                 len(signal_list), path_to_assign_list
             )
         )
 
         if len(signal_list) == 0:
-            self.logger.error(
-                "Could not load bit assign list: {}".format(path_to_assign_list)
-            )
+            self.logger.error("Could not load bit assign list: {}".format(path_to_assign_list))
             sys.exit(1)
 
     def bit_assigns_from_can_id(self, can_id):
         """Returns list of bit assign information which corresponds to the given CAN ID.
 
         Args:
             can_id (str): ID of CAN
@@ -170,17 +168,15 @@
         Args:
             time_in_nsec (str): Time in nano-seconds
             data_label (str): Data label
             data (str): Data
 
         """
         self.time_in_nsec = time_in_nsec
-        self.time_in_datetime = datetime.datetime.fromtimestamp(
-            float(time_in_nsec) / 1.0e9
-        )
+        self.time_in_datetime = datetime.datetime.fromtimestamp(float(time_in_nsec) / 1.0e9)
         self.data_label = data_label
         self.data = data
 
 
 class CANDecoder(object):
     """CAN csv file decoder."""
 
@@ -260,17 +256,15 @@
         row = next(self.reader)
         if not row:
             raise EOFError
 
         # Analyze
         for bit_assign in self.bit_assign_info.bit_assigns_from_can_id(row[1]):
             data.append(
-                CANData(
-                    row[0], bit_assign.data_label, self.unpack_data(row[3], bit_assign)
-                )
+                CANData(row[0], bit_assign.data_label, self.unpack_data(row[3], bit_assign))
             )
 
         return data
 
     def analyze_csv(self, path_to_csv="", start_time=None, end_time=None):
         """Returns list of CANData.
 
@@ -303,24 +297,19 @@
         with open(path_to_csv, "rU") as f:
             reader = csv.reader(f)
             _ = next(reader)  # Header
 
             for row in reader:
                 timestamp = row[2]
                 can_id = (
-                    bitstring.ConstBitArray(uint=int(row[5]), length=32)
-                    .hex.lstrip("0")
-                    .lower()
+                    bitstring.ConstBitArray(uint=int(row[5]), length=32).hex.lstrip("0").lower()
                 )
                 _ = int(row[6])  # can_length
                 can_data = "".join(
-                    [
-                        bitstring.ConstBitArray(uint=int(b), length=8).hex
-                        for b in row[7:15]
-                    ]
+                    [bitstring.ConstBitArray(uint=int(b), length=8).hex for b in row[7:15]]
                 )
                 for bit_assign in self.bit_assign_info.bit_assigns_from_can_id(can_id):
                     data.append(
                         CANData(
                             timestamp,
                             bit_assign.data_label,
                             self.unpack_data(can_data, bit_assign),
@@ -329,17 +318,15 @@
                 if line_index % 500000 == 0:
                     self.logger.debug("{} lines decoded".format(line_index))
                 line_index += 1
 
         # check
         if line_datetime is not None and line_datetime < end_time:
             self.logger.error(
-                "This csv file ends {0} before end_time {1}".format(
-                    line_datetime, end_time
-                )
+                "This csv file ends {0} before end_time {1}".format(line_datetime, end_time)
             )
             return []
 
         # return
         return data
 
     @staticmethod
@@ -360,26 +347,22 @@
             data_position_2 = int(bit_assign.data_position.split(".")[1])
         else:
             data_position_1 = int(bit_assign.data_position)
             data_position_2 = 0
         start_position = data_position_1 * 8 - data_position_2
         data_len = int(bit_assign.data_length)  # bits
 
-        data = bitstring.ConstBitArray(
-            bin=c.bin[(start_position - data_len) : start_position]
-        )
+        data = bitstring.ConstBitArray(bin=c.bin[(start_position - data_len) : start_position])
 
         if bit_assign.signed == "1":
             base_value = data.int
         else:
             base_value = data.uint
 
-        value = base_value * float(bit_assign.resolution) + float(
-            bit_assign.offset_physical
-        )
+        value = base_value * float(bit_assign.resolution) + float(bit_assign.offset_physical)
 
         return value
 
 
 class CANDeserializer(object):
     """Deserialize CAN data."""
 
@@ -387,17 +370,15 @@
         """Initialize CANDeserializer.
 
         Args:
             signal_list (list): A list of signals (str) to deserialize
 
         """
         self.logger = logging.getLogger(type(self).__name__)
-        self.signal_list = (
-            ["brake_pos", "turn_signal"] if signal_list is None else signal_list
-        )
+        self.signal_list = ["brake_pos", "turn_signal"] if signal_list is None else signal_list
 
     def deserialize(self, can_data, start_time=None, end_time=None, fps=5):
         """Deserializes given CAN data from start_time to end_time with given fps.
 
         Args:
             can_data (list): A list of CANData objects
             start_time (datetime): Start-time to deserialize data
@@ -419,45 +400,40 @@
 
         if end_time is None:
             end_time = can_data[-1].time_in_datetime
             self.logger.debug("setting end_time as: {}".format(end_time))
 
         # prepare
         current_time_start = start_time
-        current_time_end = start_time + datetime.timedelta(
-            seconds=(float(1.0) / float(fps))
-        )
+        current_time_end = start_time + datetime.timedelta(seconds=(float(1.0) / float(fps)))
         current_index = 0
         # end_of_data_flag = False
 
         # prepare tables
         previous = {signal: None for signal in self.signal_list}
         result = {signal: [] for signal in self.signal_list}
         result["time_in_datetime"] = []
 
         # loop
         self.logger.debug("started can data deserialization")
         while current_index < len(can_data):
-
             # initialize signal_temp dictionary
             signal_temp = {signal: [] for signal in self.signal_list}
             signal_temp_previous = {signal: [] for signal in self.signal_list}
 
             # store can signals
             for can_signal in can_data[current_index:]:
                 if current_time_start <= can_signal.time_in_datetime < current_time_end:
                     if can_signal.data_label in self.signal_list:
                         signal_temp[can_signal.data_label].append(can_signal.data)
                     current_index += 1
                 else:
                     if can_signal.time_in_datetime < current_time_start:
                         if can_signal.data_label in self.signal_list:
-                            signal_temp_previous[can_signal.data_label].append(
-                                can_signal.data
-                            )
+                            signal_temp_previous[can_signal.data_label].append(can_signal.data)
                         current_index += 1
                     elif can_signal.time_in_datetime > current_time_end:
                         break
 
             # calculate average and store it
             for signal in self.signal_list:
                 # store previous signals if exists
@@ -515,39 +491,28 @@
         logging.basicConfig(level=logging.WARNING)
 
     can_decoder = CANDecoder(args.assign_list)
     can_data = can_decoder.analyze_csv(args.path_to_csv)
 
     if args.verbose:
         for data in can_data:
-            print(
-                "{0}, {1}, {2}".format(
-                    data.unix_time_in_millisecond, data.data_label, data.data
-                )
-            )
+            print("{0}, {1}, {2}".format(data.unix_time_in_millisecond, data.data_label, data.data))
 
     can_deserializer = CANDeserializer()
     signal_list = can_deserializer.signal_list
     can_data_deserialized = can_deserializer.deserialize(can_data, fps=10)
 
     # print
-    print(
-        "{0:>20},{1}".format(
-            "Timestamp", ",".join(["{0:>16}".format(k) for k in signal_list])
-        )
-    )
+    print("{0:>20},{1}".format("Timestamp", ",".join(["{0:>16}".format(k) for k in signal_list])))
     for idx, stamp in enumerate(can_data_deserialized["time_in_datetime"]):
         print(
             "{0:>20},{1}".format(
                 str(int(time.mktime(stamp.timetuple()))) + stamp.strftime("%f000"),
                 ",".join(
-                    [
-                        "{0:>16,.03f}".format(can_data_deserialized[k][idx])
-                        for k in signal_list
-                    ]
+                    ["{0:>16,.03f}".format(can_data_deserialized[k][idx]) for k in signal_list]
                 ),
             )
         )
 
 
 if __name__ == "__main__":
     # parser
```

### Comparing `pydtk-0.2.9/pydtk/utils/fileutils.py` & `pydtk-0.3.0/pydtk/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.9/pydtk/utils/utils.py` & `pydtk-0.3.0/pydtk/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,15 @@
         name (str): name of config (e.g. 'v1')
 
     Returns:
         (AttrDict): config
 
     """
     with open(
-        os.path.join(
-            os.path.dirname(os.path.dirname(__file__)), "conf", name + ".yaml"
-        ),
+        os.path.join(os.path.dirname(os.path.dirname(__file__)), "conf", name + ".yaml"),
         "r",
     ) as f:
         config = yaml.load(f, Loader=yaml.SafeLoader)
     return AttrDict(config)
 
 
 def tag_filter(tag_list, base_df):
@@ -102,17 +100,15 @@
         file_df (DataFrame): Search target.
 
     Returns:
         start_timestamp (float)
         end_timestamp (float)
 
     """
-    mask = (file_df["start_timestamp"] != "no info") & (
-        file_df["start_timestamp"] != "Nan"
-    )
+    mask = (file_df["start_timestamp"] != "no info") & (file_df["start_timestamp"] != "Nan")
     start_timestamp = file_df[mask]["start_timestamp"].max()
     mask = (file_df["end_timestamp"] != "no info") & (file_df["end_timestamp"] != "Nan")
     end_timestamp = file_df[mask]["end_timestamp"].min()
 
     return start_timestamp, end_timestamp
 
 
@@ -310,14 +306,15 @@
     Args:
         func (function): a function whose arguments should be checked
 
     Returns:
         function: decorated function
 
     """
+
     def fix(*args, **kwargs):
         """Fix arguments type."""
         if "database_id" in kwargs.keys():
             kwargs["database_id"] = str(kwargs["database_id"])
         func(*args, **kwargs)
 
     return fix
```

### Comparing `pydtk-0.2.9/pyproject.toml` & `pydtk-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry >= 1.0.0", "setuptools >= 50.3.0", "wheel >= 0.35.1", "pip >= 21.0.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pydtk"
-version = "0.2.9"
+version = "0.3.0"
 description = "A Python toolkit for managing, retrieving and processing data."
 license = "Apache-2.0"
 authors = [
     "Yusuke Adachi <adachi.yusuke@hdwlab.co.jp>",
     "Daiki Hayashi <hayashi.daiki@hdwlab.co.jp>",
     "Toshimitsu Watanabe <watanabe.toshimitsu@hdwlab.co.jp>"
 ]
@@ -49,14 +49,15 @@
 montydb = {extras = ["bson", "lmdb"], version = "^2.4.0"}
 flatdict = { version = "^4.0.1", optional = true }
 pyzstd = { version = "^0.15.0", optional = true }
 pydantic = "^1.10.2"
 lark =  { version = "^1.1.5", optional = true }
 scipy = "^1.8.0"
 addict = "^2.4.0"
+iso8601 = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
 importlib-resources = "<2.0.0"
 importlib-metadata = "<2.0.0"
 pytest = "^6.0.0"
 flake8-docstrings = "^1.5.0"
 tox = "<=3.17.0"
@@ -78,7 +79,18 @@
 batch_analyze_statistics = "pydtk.builder.statistic_db:batch_script"
 make_meta = "pydtk.bin.make_meta:main"
 pydtk = "pydtk.bin.cli:script"
 oas_dump = "pydtk.bin.oas:script"
 
 [tool.pytest.ini_options]
 markers = ["extra", "ros", "ros2", "cassandra", "pointcloud", "zstd"]
+
+# NOTE(kan-bayashi): black does not support tox.ini
+[tool.black]
+line-length = 100
+extend-exclude = '''
+/(
+  | .venv
+  | .pytest_cache
+  | openapi
+)/
+'''
```

### Comparing `pydtk-0.2.9/PKG-INFO` & `pydtk-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: pydtk
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Python toolkit for managing, retrieving and processing data.
 Home-page: https://github.com/dataware-tools/python-toolkit.git
 License: Apache-2.0
 Keywords: toolkit,data,dataware,metadata
 Author: Yusuke Adachi
 Author-email: adachi.yusuke@hdwlab.co.jp
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: pointcloud
 Provides-Extra: ros
 Provides-Extra: ros2
 Provides-Extra: zstd
 Requires-Dist: addict (>=2.4.0,<3.0.0)
 Requires-Dist: bitstring (>=3.1.7,<4.0.0)
 Requires-Dist: deepmerge (>=0.1.1,<0.2.0)
 Requires-Dist: fire (>=0.3.1,<0.4.0)
-Requires-Dist: flatdict (>=4.0.1,<5.0.0); extra == "ros" or extra == "ros2"
+Requires-Dist: flatdict (>=4.0.1,<5.0.0) ; extra == "ros" or extra == "ros2"
 Requires-Dist: flatten-dict (>=0.3.0,<0.4.0)
-Requires-Dist: gnupg; extra == "ros"
-Requires-Dist: lark (>=1.1.5,<2.0.0); extra == "ros2"
-Requires-Dist: montydb[lmdb,bson] (>=2.4.0,<3.0.0)
+Requires-Dist: gnupg ; extra == "ros"
+Requires-Dist: iso8601 (>=1.1.0,<2.0.0)
+Requires-Dist: lark (>=1.1.5,<2.0.0) ; extra == "ros2"
+Requires-Dist: montydb[bson,lmdb] (>=2.4.0,<3.0.0)
 Requires-Dist: numpy (<1.24.0)
 Requires-Dist: opencv-python (>=4.2.0.34,<5.0.0.0)
 Requires-Dist: pandas (>=1.0.3,<2.0.0)
-Requires-Dist: pycryptodomex; extra == "ros"
+Requires-Dist: pycryptodomex ; extra == "ros"
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pymongo (>=3.11.3,<4.0.0)
-Requires-Dist: pyntcloud; extra == "pointcloud"
+Requires-Dist: pyntcloud ; extra == "pointcloud"
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pyyaml
-Requires-Dist: pyzstd (>=0.15.0,<0.16.0); extra == "zstd"
-Requires-Dist: rospkg; extra == "ros"
+Requires-Dist: pyzstd (>=0.15.0,<0.16.0) ; extra == "zstd"
+Requires-Dist: rospkg ; extra == "ros"
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: six (>=1.15.0,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.3.17,<2.0.0)
 Requires-Dist: sqlalchemy-migrate
 Requires-Dist: tinydb (>=3.2.1,<4.0.0)
 Requires-Dist: tinymongo (>=0.2.0,<0.3.0)
 Requires-Dist: tqdm (>=4.46.1,<5.0.0)
@@ -56,15 +57,15 @@
 ## Installation
 You can install the toolkit with:
 ```bash
 $ pip3 install pydtk
 
 ```
 
-If you want to install the toolkit with extra feature (e.g. support for PointCloud and ROS), 
+If you want to install the toolkit with extra feature (e.g. support for PointCloud and ROS),
 you can install it with extra dependencies as follows:
 ```bash
 $ pip3 install pydtk[pointcloud,ros]
 
 ```
 
 Some PyDTK models require additional packages.  
@@ -126,26 +127,26 @@
 
 
 ## Documentation
 For more information about this toolkit, please refer the [document](https://dataware-tools.github.io/pydtk/).
 
 
 ## Setup for contribution
-To improve this toolkit, firstly clone this repository and then 
-run the following command to prepare the environment. 
+To improve this toolkit, firstly clone this repository and then
+run the following command to prepare the environment.
 
 ```bash
 $ git clone git@github.com:dataware-tools/pydtk.git --recurse-submodules
 $ poetry install
 
 ```
 
 Make sure that [poetry](https://python-poetry.org/) is installed before executing the command.
 
-If you want to install the toolkit with extra feature (e.g. support for ROS), 
+If you want to install the toolkit with extra feature (e.g. support for ROS),
 please specify it with `-E` option.  
 Example (installation with `pointcloud` and `ros` extras):
 ```bash
 $ poetry install -E pointcloud -E ros
 
 ```
```

