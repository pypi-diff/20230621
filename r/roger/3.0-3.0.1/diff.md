# Comparing `tmp/roger-3.0.tar.gz` & `tmp/roger-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roger-3.0.tar", last modified: Sun Feb 12 14:19:42 2023, max compression
+gzip compressed data, was "roger-3.0.1.tar", last modified: Wed Jun 21 15:35:09 2023, max compression
```

## Comparing `roger-3.0.tar` & `roger-3.0.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.705093 roger-3.0/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1072 2023-01-28 18:10:37.000000 roger-3.0/LICENSE
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      521 2023-02-10 12:04:56.000000 roger-3.0/MANIFEST.in
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6978 2023-02-12 14:19:42.706682 roger-3.0/PKG-INFO
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5864 2023-02-10 20:42:33.000000 roger-3.0/README.md
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4083 2023-01-28 18:10:37.000000 roger-3.0/cuda_ext.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.487710 roger-3.0/look_up_tables/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     9303 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/crop_parameters.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     1174 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/intercept_land_use.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      818 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/intercept_sealing.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     3122 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/mp_drain_area.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)   587663 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/mp_layer_manning_strickler.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      672 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/root_depth_land_use.csv
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      247 2023-01-28 18:10:43.000000 roger-3.0/pyproject.toml
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      186 2023-02-10 15:42:45.000000 roger-3.0/requirements.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       27 2023-02-08 17:52:32.000000 roger-3.0/requirements_jax.txt
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.739269 roger-3.0/roger/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2354 2023-01-28 18:10:43.000000 roger-3.0/roger/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      495 2023-02-12 14:19:42.739524 roger-3.0/roger/_version.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2410 2023-01-28 18:10:43.000000 roger-3.0/roger/backend.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.532441 roger-3.0/roger/cli/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      584 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      116 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3143 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_copy_model.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1045 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_create_mask.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3066 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_resubmit.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4344 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_run.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1410 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_run_base.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.563441 roger-3.0/roger/core/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1364 2023-01-28 18:10:43.000000 roger-3.0/roger/core/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    21126 2023-01-28 18:10:43.000000 roger-3.0/roger/core/adaptive_time_stepping.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    17885 2023-01-28 18:10:43.000000 roger-3.0/roger/core/capillary_rise.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    66629 2023-01-28 18:10:43.000000 roger-3.0/roger/core/crop.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    26780 2023-01-28 18:10:43.000000 roger-3.0/roger/core/evapotranspiration.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    23142 2023-01-28 18:10:43.000000 roger-3.0/roger/core/film_flow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4075 2023-01-28 18:10:43.000000 roger-3.0/roger/core/groundwater.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3592 2023-01-28 18:10:43.000000 roger-3.0/roger/core/groundwater_flow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    69882 2023-01-28 18:10:43.000000 roger-3.0/roger/core/infiltration.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13502 2023-01-28 18:10:43.000000 roger-3.0/roger/core/interception.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     9290 2023-01-28 18:10:43.000000 roger-3.0/roger/core/nitrate.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    26889 2023-01-28 18:10:43.000000 roger-3.0/roger/core/numerics.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5705 2023-01-28 18:10:43.000000 roger-3.0/roger/core/operators.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7632 2023-01-28 18:10:43.000000 roger-3.0/roger/core/root_zone.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11373 2023-01-28 18:10:43.000000 roger-3.0/roger/core/sas.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11056 2023-01-28 18:10:43.000000 roger-3.0/roger/core/snow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    46149 2023-01-28 18:10:43.000000 roger-3.0/roger/core/soil.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7656 2023-01-28 18:10:43.000000 roger-3.0/roger/core/subsoil.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    58575 2023-01-28 18:10:43.000000 roger-3.0/roger/core/subsurface_runoff.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13121 2023-01-28 18:10:43.000000 roger-3.0/roger/core/surface.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      258 2023-01-28 18:10:43.000000 roger-3.0/roger/core/surface_runoff.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)   170691 2023-01-28 18:10:43.000000 roger-3.0/roger/core/transport.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4838 2023-01-28 18:10:43.000000 roger-3.0/roger/core/utilities.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.575245 roger-3.0/roger/diagnostics/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      105 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2059 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/api.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3307 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/average.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4047 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/base.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2756 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/collect.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2790 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/constant.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3793 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/maximum.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3794 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/minimum.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2839 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/rate.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1580 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/snapshot.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1360 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/tracer_monitor.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1378 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/water_monitor.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    18158 2023-01-28 18:10:43.000000 roger-3.0/roger/distributed.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.582122 roger-3.0/roger/io_tools/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6124 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/csv.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1660 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/hdf5.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6257 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/netcdf.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      522 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/yml.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1907 2023-01-28 18:10:43.000000 roger-3.0/roger/logs.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2576 2023-01-28 18:10:43.000000 roger-3.0/roger/lookuptables.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.583876 roger-3.0/roger/models/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/models/__init__.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.585542 roger-3.0/roger/models/dummy/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-01-28 18:10:43.000000 roger-3.0/roger/models/dummy/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1251 2023-01-28 18:10:43.000000 roger-3.0/roger/models/dummy/dummy.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.590098 roger-3.0/roger/models/oneD/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0/roger/models/oneD/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13312 2023-01-28 18:10:43.000000 roger-3.0/roger/models/oneD/oneD.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.593186 roger-3.0/roger/models/oneD_event/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       76 2023-01-28 18:10:43.000000 roger-3.0/roger/models/oneD_event/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11459 2023-01-28 18:10:43.000000 roger-3.0/roger/models/oneD_event/oneD_event.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.595985 roger-3.0/roger/models/svat/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11572 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat/svat.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.600371 roger-3.0/roger/models/svat_bromide/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       84 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_bromide/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14478 2023-02-08 16:26:37.000000 roger-3.0/roger/models/svat_bromide/svat_bromide.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.604427 roger-3.0/roger/models/svat_crop/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       73 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    16051 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop/svat_crop.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.607837 roger-3.0/roger/models/svat_crop_bromide/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop_bromide/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop_bromide/svat_crop_bromide.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.611148 roger-3.0/roger/models/svat_crop_nitrate/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop_nitrate/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop_nitrate/svat_crop_nitrate.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.613200 roger-3.0/roger/models/svat_oxygen18/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       86 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_oxygen18/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    19035 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_oxygen18/svat_oxygen18.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1936 2023-01-28 18:10:43.000000 roger-3.0/roger/plugins.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6475 2023-01-28 18:10:43.000000 roger-3.0/roger/progress.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6221 2023-01-28 18:10:43.000000 roger-3.0/roger/restart.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    25023 2023-01-28 18:10:43.000000 roger-3.0/roger/roger.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14190 2023-01-28 18:10:43.000000 roger-3.0/roger/routines.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5954 2023-01-28 18:10:43.000000 roger-3.0/roger/runtime.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     9218 2023-02-11 12:18:32.000000 roger-3.0/roger/settings.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2330 2023-01-28 18:10:43.000000 roger-3.0/roger/signals.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    17650 2023-01-28 18:10:43.000000 roger-3.0/roger/state.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      819 2023-01-28 18:10:43.000000 roger-3.0/roger/time.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      451 2023-01-28 18:10:43.000000 roger-3.0/roger/timer.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.630768 roger-3.0/roger/tools/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    31909 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/evaluation.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    20672 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/event_classification.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    12678 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/filelock.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14559 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/labels.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    24578 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/make_toy_data.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      134 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/plotting.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    22516 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/setup.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)   176931 2023-01-28 18:10:43.000000 roger-3.0/roger/variables.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.525638 roger-3.0/roger.egg-info/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6978 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/PKG-INFO
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3170 2023-02-12 14:19:42.000000 roger-3.0/roger.egg-info/SOURCES.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/dependency_links.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      270 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/entry_points.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2023-02-10 15:15:06.000000 roger-3.0/roger.egg-info/not-zip-safe
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      291 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/requires.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       11 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/top_level.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      327 2023-02-12 14:19:42.730873 roger-3.0/setup.cfg
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4627 2023-02-10 16:39:56.000000 roger-3.0/setup.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.699889 roger-3.0/test/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      103 2023-02-08 16:07:16.000000 roger-3.0/test/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1075 2023-01-28 18:10:43.000000 roger-3.0/test/cli_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      391 2023-02-08 13:33:29.000000 roger-3.0/test/conftest.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    23321 2023-02-08 17:11:16.000000 roger-3.0/test/make_data_for_svat_transport.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1076 2023-02-08 18:10:29.000000 roger-3.0/test/progress_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2684 2023-01-28 18:10:43.000000 roger-3.0/test/restart_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5047 2023-02-08 17:11:11.000000 roger-3.0/test/setup_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3320 2023-02-08 13:27:57.000000 roger-3.0/test/state_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    68611 2023-01-28 18:10:43.000000 roger-3.0/versioneer.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.449859 roger-3.0.1/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1072 2023-01-28 18:10:37.000000 roger-3.0.1/LICENSE
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      521 2023-02-10 12:04:56.000000 roger-3.0.1/MANIFEST.in
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7024 2023-06-21 15:35:09.449961 roger-3.0.1/PKG-INFO
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5908 2023-02-23 16:39:50.000000 roger-3.0.1/README.md
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4083 2023-01-28 18:10:37.000000 roger-3.0.1/cuda_ext.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.417400 roger-3.0.1/look_up_tables/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     9303 2023-01-28 18:10:43.000000 roger-3.0.1/look_up_tables/crop_parameters.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     1174 2023-01-28 18:10:43.000000 roger-3.0.1/look_up_tables/intercept_land_use.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      818 2023-01-28 18:10:43.000000 roger-3.0.1/look_up_tables/intercept_sealing.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     3122 2023-01-28 18:10:43.000000 roger-3.0.1/look_up_tables/mp_drain_area.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)   587663 2023-01-28 18:10:43.000000 roger-3.0.1/look_up_tables/mp_layer_manning_strickler.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      672 2023-01-28 18:10:43.000000 roger-3.0.1/look_up_tables/root_depth_land_use.csv
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      231 2023-06-21 07:35:40.000000 roger-3.0.1/pyproject.toml
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      187 2023-05-11 09:45:24.000000 roger-3.0.1/requirements.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       25 2023-06-20 14:00:41.000000 roger-3.0.1/requirements_jax.txt
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.450452 roger-3.0.1/roger/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2354 2023-01-28 18:10:43.000000 roger-3.0.1/roger/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      497 2023-06-21 15:35:09.450493 roger-3.0.1/roger/_version.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2410 2023-01-28 18:10:43.000000 roger-3.0.1/roger/backend.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.426875 roger-3.0.1/roger/cli/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      584 2023-01-28 18:10:43.000000 roger-3.0.1/roger/cli/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      116 2023-01-28 18:10:43.000000 roger-3.0.1/roger/cli/roger.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3143 2023-01-28 18:10:43.000000 roger-3.0.1/roger/cli/roger_copy_model.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1045 2023-01-28 18:10:43.000000 roger-3.0.1/roger/cli/roger_create_mask.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3066 2023-01-28 18:10:43.000000 roger-3.0.1/roger/cli/roger_resubmit.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4344 2023-01-28 18:10:43.000000 roger-3.0.1/roger/cli/roger_run.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1410 2023-01-28 18:10:43.000000 roger-3.0.1/roger/cli/roger_run_base.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.436958 roger-3.0.1/roger/core/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1364 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    12901 2023-04-06 14:51:02.000000 roger-3.0.1/roger/core/adaptive_time_stepping.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    17885 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/capillary_rise.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    69903 2023-06-19 08:42:59.000000 roger-3.0.1/roger/core/crop.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    26821 2023-05-16 09:37:57.000000 roger-3.0.1/roger/core/evapotranspiration.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    23142 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/film_flow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4075 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/groundwater.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3592 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/groundwater_flow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    69882 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/infiltration.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13502 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/interception.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     9290 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/nitrate.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    38933 2023-06-20 13:12:22.000000 roger-3.0.1/roger/core/numerics.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5705 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/operators.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7662 2023-06-14 14:01:14.000000 roger-3.0.1/roger/core/root_zone.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11373 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/sas.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11056 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/snow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    45990 2023-06-15 12:29:42.000000 roger-3.0.1/roger/core/soil.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7686 2023-06-13 16:12:33.000000 roger-3.0.1/roger/core/subsoil.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    58703 2023-05-15 10:05:36.000000 roger-3.0.1/roger/core/subsurface_runoff.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13121 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/surface.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      258 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/surface_runoff.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)   175121 2023-06-13 10:28:36.000000 roger-3.0.1/roger/core/transport.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4838 2023-01-28 18:10:43.000000 roger-3.0.1/roger/core/utilities.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.439899 roger-3.0.1/roger/diagnostics/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      105 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2059 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/api.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3307 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/average.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4047 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/base.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2756 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/collect.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2790 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/constant.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3793 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/maximum.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3794 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/minimum.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2839 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/rate.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1580 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/snapshot.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1360 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/tracer_monitor.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1378 2023-01-28 18:10:43.000000 roger-3.0.1/roger/diagnostics/water_monitor.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    18158 2023-01-28 18:10:43.000000 roger-3.0.1/roger/distributed.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.441324 roger-3.0.1/roger/io_tools/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.1/roger/io_tools/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6124 2023-01-28 18:10:43.000000 roger-3.0.1/roger/io_tools/csv.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1660 2023-01-28 18:10:43.000000 roger-3.0.1/roger/io_tools/hdf5.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6257 2023-01-28 18:10:43.000000 roger-3.0.1/roger/io_tools/netcdf.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      522 2023-01-28 18:10:43.000000 roger-3.0.1/roger/io_tools/yml.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1907 2023-01-28 18:10:43.000000 roger-3.0.1/roger/logs.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2576 2023-01-28 18:10:43.000000 roger-3.0.1/roger/lookuptables.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.441557 roger-3.0.1/roger/models/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/__init__.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.442038 roger-3.0.1/roger/models/dummy/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/dummy/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1251 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/dummy/dummy.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.442608 roger-3.0.1/roger/models/oneD/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/oneD/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13312 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/oneD/oneD.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.443170 roger-3.0.1/roger/models/oneD_event/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       76 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/oneD_event/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11459 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/oneD_event/oneD_event.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.443668 roger-3.0.1/roger/models/svat/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11572 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat/svat.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.444035 roger-3.0.1/roger/models/svat_bromide/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       84 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat_bromide/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14478 2023-02-08 16:26:37.000000 roger-3.0.1/roger/models/svat_bromide/svat_bromide.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.444401 roger-3.0.1/roger/models/svat_crop/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       73 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat_crop/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    16382 2023-06-15 12:30:32.000000 roger-3.0.1/roger/models/svat_crop/svat_crop.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.444919 roger-3.0.1/roger/models/svat_crop_bromide/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat_crop_bromide/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat_crop_bromide/svat_crop_bromide.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.445238 roger-3.0.1/roger/models/svat_crop_nitrate/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat_crop_nitrate/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat_crop_nitrate/svat_crop_nitrate.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.445548 roger-3.0.1/roger/models/svat_oxygen18/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       86 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat_oxygen18/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    19035 2023-01-28 18:10:43.000000 roger-3.0.1/roger/models/svat_oxygen18/svat_oxygen18.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1936 2023-01-28 18:10:43.000000 roger-3.0.1/roger/plugins.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6475 2023-01-28 18:10:43.000000 roger-3.0.1/roger/progress.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6221 2023-01-28 18:10:43.000000 roger-3.0.1/roger/restart.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    25235 2023-06-15 09:11:18.000000 roger-3.0.1/roger/roger.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14190 2023-01-28 18:10:43.000000 roger-3.0.1/roger/routines.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5954 2023-01-28 18:10:43.000000 roger-3.0.1/roger/runtime.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     9218 2023-02-11 12:18:32.000000 roger-3.0.1/roger/settings.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2330 2023-01-28 18:10:43.000000 roger-3.0.1/roger/signals.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    17650 2023-01-28 18:10:43.000000 roger-3.0.1/roger/state.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      828 2023-05-16 09:12:42.000000 roger-3.0.1/roger/time.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      451 2023-01-28 18:10:43.000000 roger-3.0.1/roger/timer.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.447479 roger-3.0.1/roger/tools/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.1/roger/tools/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    31911 2023-03-09 16:53:28.000000 roger-3.0.1/roger/tools/evaluation.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    20672 2023-01-28 18:10:43.000000 roger-3.0.1/roger/tools/event_classification.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    12678 2023-01-28 18:10:43.000000 roger-3.0.1/roger/tools/filelock.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14598 2023-03-09 14:58:18.000000 roger-3.0.1/roger/tools/labels.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    24578 2023-01-28 18:10:43.000000 roger-3.0.1/roger/tools/make_toy_data.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      134 2023-01-28 18:10:43.000000 roger-3.0.1/roger/tools/plotting.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    22516 2023-05-16 12:52:16.000000 roger-3.0.1/roger/tools/setup.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)   181145 2023-06-19 11:22:43.000000 roger-3.0.1/roger/variables.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.425074 roger-3.0.1/roger.egg-info/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7024 2023-06-21 15:35:08.000000 roger-3.0.1/roger.egg-info/PKG-INFO
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3170 2023-06-21 15:35:09.000000 roger-3.0.1/roger.egg-info/SOURCES.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2023-06-21 15:35:08.000000 roger-3.0.1/roger.egg-info/dependency_links.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      270 2023-06-21 15:35:08.000000 roger-3.0.1/roger.egg-info/entry_points.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2023-06-21 15:35:07.000000 roger-3.0.1/roger.egg-info/not-zip-safe
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      290 2023-06-21 15:35:08.000000 roger-3.0.1/roger.egg-info/requires.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       11 2023-06-21 15:35:08.000000 roger-3.0.1/roger.egg-info/top_level.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      333 2023-06-21 15:35:09.450310 roger-3.0.1/setup.cfg
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4627 2023-02-10 16:39:56.000000 roger-3.0.1/setup.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-06-21 15:35:09.449685 roger-3.0.1/test/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      103 2023-02-08 16:07:16.000000 roger-3.0.1/test/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1075 2023-01-28 18:10:43.000000 roger-3.0.1/test/cli_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      391 2023-02-08 13:33:29.000000 roger-3.0.1/test/conftest.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    23321 2023-02-08 17:11:16.000000 roger-3.0.1/test/make_data_for_svat_transport.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1065 2023-04-20 09:13:19.000000 roger-3.0.1/test/progress_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2684 2023-01-28 18:10:43.000000 roger-3.0.1/test/restart_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5047 2023-02-08 17:11:11.000000 roger-3.0.1/test/setup_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3320 2023-02-08 13:27:57.000000 roger-3.0.1/test/state_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    68611 2023-01-28 18:10:43.000000 roger-3.0.1/versioneer.py
```

### Comparing `roger-3.0/LICENSE` & `roger-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roger-3.0/MANIFEST.in` & `roger-3.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `roger-3.0/PKG-INFO` & `roger-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roger
-Version: 3.0
+Version: 3.0.1
 Summary: Runoff Generation Research - a hydrologic toolbox in Python
 Home-page: https://roger.readthedocs.io
 Author: Robin Schwemmle (University of Freiburg)
 Author-email: robin.schwemmle@hydrology.uni-freiburg.de
 License: MIT
 Keywords: hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax
 Classifier: Development Status :: 4 - Beta
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 <p align="center">
 <img src="doc/_images/roger-logo.png">
 </p>
 
 <p align="center">
-<i>Runoff Generation Research - a hydrologic toolbox in Python</i>
+<i>Runoff Generation Research - a process-based hydrological toolbox model in Python</i>
 </p>
 
 <p align="center">
   <a href="http://roger.readthedocs.io/?badge=latest">
     <img src="https://readthedocs.org/projects/roger/badge/?version=latest" alt="Documentation status">
   </a>
   <a href="https://github.com/Hydrology-IFH/roger/actions/workflows/test-all.yml">
@@ -43,17 +43,17 @@
   </a>
   <a href="https://codecov.io/gh/Hydrology-IFH/roger" > 
   <img src="https://codecov.io/gh/Hydrology-IFH/roger/branch/main/graph/badge.svg?token=KXSVNGDDNH"/> 
   </a>
   <a href="https://zenodo.org/badge/latestdoi/536477819"><img src="https://zenodo.org/badge/536477819.svg" alt="DOI"></a>
 </p>
 
-Roger, *Runoff Generation Research*, is a process-based hydrologic model that can be applied from plot to catchment scale. Roger is written in pure Python, which facilitates model setup and model workflows. We want to enable high-performance hydrologic modelling with a clear focus on flexibility and usability.
+RoGeR, *Runoff Generation Research*, is a process-based hydrological model that can be applied from plot to catchment scale. RoGeR is written in pure Python, which facilitates model setup and model workflows. We want to enable high-performance hydrologic modelling with a clear focus on flexibility and usability.
 
-Roger supports a NumPy backend for small-scale problems, and a
+RoGeR supports a NumPy backend for small-scale problems, and a
 high-performance [JAX](https://github.com/google/jax) backend
 with CPU and GPU support. Parallel computation is available via MPI and supports
 distributed execution on any number of nodes/CPU cores.
 
 Inspired by [Veros](https://veros.readthedocs.io/en/latest/).
 
 ## Documentation
@@ -136,15 +136,15 @@
 
 ## How to cite
 
 If you use Roger in scientific work, please consider citing [the following publication](...):
 
 ```bibtex
 @article{
-	title = {Roger v3.0 – a hydrologic toolbox in {Python}},
+	title = {Roger v3.0 – a process-based hydrologic toolbox model in {Python}},
 	volume = {...},
 	doi = {https://doi.org/10.5194/gmd-xxx},
 	journal = {Geosci. Model Dev.},
 	author = {Schwemmle, Robin, and Leistert, Hannes, and Weiler, Markus},
 	year = {2023},
 	pages = {...},
 }
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roger Version: 3.0 Summary: Runoff Generation
+Metadata-Version: 2.1 Name: roger Version: 3.0.1 Summary: Runoff Generation
 Research - a hydrologic toolbox in Python Home-page: https://
 roger.readthedocs.io Author: Robin Schwemmle (University of Freiburg) Author-
 email: robin.schwemmle@hydrology.uni-freiburg.de License: MIT Keywords:
 hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -10,22 +10,23 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX Classifier: Operating System :: Unix Classifier: Operating
 System :: MacOS Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: test Provides-Extra: jax License-File: LICENSE
                          [doc/_images/roger-logo.png]
-          Runoff Generation Research - a hydrologic toolbox in Python
+  Runoff Generation Research - a process-based hydrological toolbox model in
+                                    Python
   [Documentation_status] [Test_status] [https://codecov.io/gh/Hydrology-IFH/
            roger/branch/main/graph/badge.svg?token=KXSVNGDDNH] [DOI]
-Roger, *Runoff Generation Research*, is a process-based hydrologic model that
-can be applied from plot to catchment scale. Roger is written in pure Python,
+RoGeR, *Runoff Generation Research*, is a process-based hydrological model that
+can be applied from plot to catchment scale. RoGeR is written in pure Python,
 which facilitates model setup and model workflows. We want to enable high-
 performance hydrologic modelling with a clear focus on flexibility and
-usability. Roger supports a NumPy backend for small-scale problems, and a high-
+usability. RoGeR supports a NumPy backend for small-scale problems, and a high-
 performance [JAX](https://github.com/google/jax) backend with CPU and GPU
 support. Parallel computation is available via MPI and supports distributed
 execution on any number of nodes/CPU cores. Inspired by [Veros](https://
 veros.readthedocs.io/en/latest/). ## Documentation We strongly recommend to
 [visit our documentation](https://roger.readthedocs.io/en/latest/). ## Features
                     [25_square_meter_resolved_simulations_
                     of_a_rectangular_soil_covered_by_grass]
@@ -62,23 +63,23 @@
 some tips on testing and benchmarking, and to make sure that your modifications
 adhere with our style policies. Most importantly, please ensure that you follow
 the [PEP8 guidelines](https://www.python.org/dev/peps/pep-0008/), use
 *meaningful* variable names, and document your code using [Google-style
 docstrings](http://sphinxcontrib-napoleon.readthedocs.io/en/latest/
 example_google.html). ## How to cite If you use Roger in scientific work,
 please consider citing [the following publication](...): ```bibtex @article
-{ title = {Roger v3.0 â a hydrologic toolbox in {Python}}, volume = {...},
-doi = {https://doi.org/10.5194/gmd-xxx}, journal = {Geosci. Model Dev.}, author
-= {Schwemmle, Robin, and Leistert, Hannes, and Weiler, Markus}, year = {2023},
-pages = {...}, } ``` Or have a look at [our documentation](https://
-roger.readthedocs.io/en/latest/more/publications.html) for more publications
-involving Roger. ## TODO - implement runoff and channel routing (e.g. kinematic
-wave or hydraulic approach) - implement distributed model with run-on
-infiltration - use coarser spatial and temporal resolution for computation of
-groundwater-related processes - implement baseflow in the groundwater routine.
-requires surface water depth. - implement surface runoff generation for
-gravity-driven infiltration - implement gravity-driven infiltration and
-percolation and include it into the transport routine - implement time-variant
-sowing and harvesting of crops ## License This software can be distributed
-freely under the MIT license. Please read the LICENSE for further information.
-Â© 2022, Robin Schwemmle (
+{ title = {Roger v3.0 â a process-based hydrologic toolbox model in
+{Python}}, volume = {...}, doi = {https://doi.org/10.5194/gmd-xxx}, journal =
+{Geosci. Model Dev.}, author = {Schwemmle, Robin, and Leistert, Hannes, and
+Weiler, Markus}, year = {2023}, pages = {...}, } ``` Or have a look at [our
+documentation](https://roger.readthedocs.io/en/latest/more/publications.html)
+for more publications involving Roger. ## TODO - implement runoff and channel
+routing (e.g. kinematic wave or hydraulic approach) - implement distributed
+model with run-on infiltration - use coarser spatial and temporal resolution
+for computation of groundwater-related processes - implement baseflow in the
+groundwater routine. requires surface water depth. - implement surface runoff
+generation for gravity-driven infiltration - implement gravity-driven
+infiltration and percolation and include it into the transport routine -
+implement time-variant sowing and harvesting of crops ## License This software
+can be distributed freely under the MIT license. Please read the LICENSE for
+further information. Â© 2022, Robin Schwemmle (
 schwemmle@hydrology.uni-freiburg.de>)
```

### Comparing `roger-3.0/README.md` & `roger-3.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
 <img src="doc/_images/roger-logo.png">
 </p>
 
 <p align="center">
-<i>Runoff Generation Research - a hydrologic toolbox in Python</i>
+<i>Runoff Generation Research - a process-based hydrological toolbox model in Python</i>
 </p>
 
 <p align="center">
   <a href="http://roger.readthedocs.io/?badge=latest">
     <img src="https://readthedocs.org/projects/roger/badge/?version=latest" alt="Documentation status">
   </a>
   <a href="https://github.com/Hydrology-IFH/roger/actions/workflows/test-all.yml">
@@ -15,17 +15,17 @@
   </a>
   <a href="https://codecov.io/gh/Hydrology-IFH/roger" > 
   <img src="https://codecov.io/gh/Hydrology-IFH/roger/branch/main/graph/badge.svg?token=KXSVNGDDNH"/> 
   </a>
   <a href="https://zenodo.org/badge/latestdoi/536477819"><img src="https://zenodo.org/badge/536477819.svg" alt="DOI"></a>
 </p>
 
-Roger, *Runoff Generation Research*, is a process-based hydrologic model that can be applied from plot to catchment scale. Roger is written in pure Python, which facilitates model setup and model workflows. We want to enable high-performance hydrologic modelling with a clear focus on flexibility and usability.
+RoGeR, *Runoff Generation Research*, is a process-based hydrological model that can be applied from plot to catchment scale. RoGeR is written in pure Python, which facilitates model setup and model workflows. We want to enable high-performance hydrologic modelling with a clear focus on flexibility and usability.
 
-Roger supports a NumPy backend for small-scale problems, and a
+RoGeR supports a NumPy backend for small-scale problems, and a
 high-performance [JAX](https://github.com/google/jax) backend
 with CPU and GPU support. Parallel computation is available via MPI and supports
 distributed execution on any number of nodes/CPU cores.
 
 Inspired by [Veros](https://veros.readthedocs.io/en/latest/).
 
 ## Documentation
@@ -108,15 +108,15 @@
 
 ## How to cite
 
 If you use Roger in scientific work, please consider citing [the following publication](...):
 
 ```bibtex
 @article{
-	title = {Roger v3.0 – a hydrologic toolbox in {Python}},
+	title = {Roger v3.0 – a process-based hydrologic toolbox model in {Python}},
 	volume = {...},
 	doi = {https://doi.org/10.5194/gmd-xxx},
 	journal = {Geosci. Model Dev.},
 	author = {Schwemmle, Robin, and Leistert, Hannes, and Weiler, Markus},
 	year = {2023},
 	pages = {...},
 }
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
                          [doc/_images/roger-logo.png]
-          Runoff Generation Research - a hydrologic toolbox in Python
+  Runoff Generation Research - a process-based hydrological toolbox model in
+                                    Python
   [Documentation_status] [Test_status] [https://codecov.io/gh/Hydrology-IFH/
            roger/branch/main/graph/badge.svg?token=KXSVNGDDNH] [DOI]
-Roger, *Runoff Generation Research*, is a process-based hydrologic model that
-can be applied from plot to catchment scale. Roger is written in pure Python,
+RoGeR, *Runoff Generation Research*, is a process-based hydrological model that
+can be applied from plot to catchment scale. RoGeR is written in pure Python,
 which facilitates model setup and model workflows. We want to enable high-
 performance hydrologic modelling with a clear focus on flexibility and
-usability. Roger supports a NumPy backend for small-scale problems, and a high-
+usability. RoGeR supports a NumPy backend for small-scale problems, and a high-
 performance [JAX](https://github.com/google/jax) backend with CPU and GPU
 support. Parallel computation is available via MPI and supports distributed
 execution on any number of nodes/CPU cores. Inspired by [Veros](https://
 veros.readthedocs.io/en/latest/). ## Documentation We strongly recommend to
 [visit our documentation](https://roger.readthedocs.io/en/latest/). ## Features
                     [25_square_meter_resolved_simulations_
                     of_a_rectangular_soil_covered_by_grass]
@@ -47,23 +48,23 @@
 some tips on testing and benchmarking, and to make sure that your modifications
 adhere with our style policies. Most importantly, please ensure that you follow
 the [PEP8 guidelines](https://www.python.org/dev/peps/pep-0008/), use
 *meaningful* variable names, and document your code using [Google-style
 docstrings](http://sphinxcontrib-napoleon.readthedocs.io/en/latest/
 example_google.html). ## How to cite If you use Roger in scientific work,
 please consider citing [the following publication](...): ```bibtex @article
-{ title = {Roger v3.0 â a hydrologic toolbox in {Python}}, volume = {...},
-doi = {https://doi.org/10.5194/gmd-xxx}, journal = {Geosci. Model Dev.}, author
-= {Schwemmle, Robin, and Leistert, Hannes, and Weiler, Markus}, year = {2023},
-pages = {...}, } ``` Or have a look at [our documentation](https://
-roger.readthedocs.io/en/latest/more/publications.html) for more publications
-involving Roger. ## TODO - implement runoff and channel routing (e.g. kinematic
-wave or hydraulic approach) - implement distributed model with run-on
-infiltration - use coarser spatial and temporal resolution for computation of
-groundwater-related processes - implement baseflow in the groundwater routine.
-requires surface water depth. - implement surface runoff generation for
-gravity-driven infiltration - implement gravity-driven infiltration and
-percolation and include it into the transport routine - implement time-variant
-sowing and harvesting of crops ## License This software can be distributed
-freely under the MIT license. Please read the LICENSE for further information.
-Â© 2022, Robin Schwemmle (
+{ title = {Roger v3.0 â a process-based hydrologic toolbox model in
+{Python}}, volume = {...}, doi = {https://doi.org/10.5194/gmd-xxx}, journal =
+{Geosci. Model Dev.}, author = {Schwemmle, Robin, and Leistert, Hannes, and
+Weiler, Markus}, year = {2023}, pages = {...}, } ``` Or have a look at [our
+documentation](https://roger.readthedocs.io/en/latest/more/publications.html)
+for more publications involving Roger. ## TODO - implement runoff and channel
+routing (e.g. kinematic wave or hydraulic approach) - implement distributed
+model with run-on infiltration - use coarser spatial and temporal resolution
+for computation of groundwater-related processes - implement baseflow in the
+groundwater routine. requires surface water depth. - implement surface runoff
+generation for gravity-driven infiltration - implement gravity-driven
+infiltration and percolation and include it into the transport routine -
+implement time-variant sowing and harvesting of crops ## License This software
+can be distributed freely under the MIT license. Please read the LICENSE for
+further information. Â© 2022, Robin Schwemmle (
 schwemmle@hydrology.uni-freiburg.de>)
```

### Comparing `roger-3.0/cuda_ext.py` & `roger-3.0.1/cuda_ext.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/look_up_tables/crop_parameters.csv` & `roger-3.0.1/look_up_tables/crop_parameters.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0/look_up_tables/intercept_land_use.csv` & `roger-3.0.1/look_up_tables/intercept_land_use.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0/look_up_tables/intercept_sealing.csv` & `roger-3.0.1/look_up_tables/intercept_sealing.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0/look_up_tables/mp_drain_area.csv` & `roger-3.0.1/look_up_tables/mp_drain_area.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0/look_up_tables/mp_layer_manning_strickler.csv` & `roger-3.0.1/look_up_tables/mp_layer_manning_strickler.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0/look_up_tables/root_depth_land_use.csv` & `roger-3.0.1/look_up_tables/root_depth_land_use.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/__init__.py` & `roger-3.0.1/roger/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/backend.py` & `roger-3.0.1/roger/backend.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/cli/__init__.py` & `roger-3.0.1/roger/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/cli/roger_copy_model.py` & `roger-3.0.1/roger/cli/roger_copy_model.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/cli/roger_create_mask.py` & `roger-3.0.1/roger/cli/roger_create_mask.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/cli/roger_resubmit.py` & `roger-3.0.1/roger/cli/roger_resubmit.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/cli/roger_run.py` & `roger-3.0.1/roger/cli/roger_run.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/cli/roger_run_base.py` & `roger-3.0.1/roger/cli/roger_run_base.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/__init__.py` & `roger-3.0.1/roger/core/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/adaptive_time_stepping.py` & `roger-3.0.1/roger/core/adaptive_time_stepping.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,223 +1,12 @@
 from roger import roger_kernel, roger_routine, KernelOutput
 from roger.core.operators import numpy as npx, update, at
 from roger.variables import allocate
 
 
-# @roger_routine
-# def adaptive_time_stepping(state):
-#     vs = state.variables
-#     settings = state.settings
-#
-#     cond0 = (vs.prec_day[2:-2, 2:-2, :] <= 0).all() & (vs.swe[2:-2, 2:-2, vs.tau] <= 0).all() & (vs.swe_top[2:-2, 2:-2, vs.tau] <= 0).all() & (vs.ta_day[2:-2, 2:-2, :] > settings.ta_fm).all()
-#     cond00 = ((vs.prec_day[2:-2, 2:-2, :] > 0) & (vs.ta_day[2:-2, 2:-2, :] <= settings.ta_fm)).any() | ((vs.prec_day[2:-2, 2:-2, :] <= 0) & (vs.ta_day[2:-2, 2:-2, :] <= settings.ta_fm)).all()
-#     cond1 = (vs.prec_day[2:-2, 2:-2, :] > settings.hpi).any() & (vs.prec_day[2:-2, 2:-2, :] > 0).any() & (vs.ta_day[2:-2, 2:-2, :] > settings.ta_fm).any()
-#     cond2 = (vs.prec_day[2:-2, 2:-2, :] <= settings.hpi).all() & (vs.prec_day[2:-2, 2:-2, :] > 0).any() & (vs.ta_day[2:-2, 2:-2, :] > settings.ta_fm).any()
-#     cond3 = (vs.prec_day[2:-2, 2:-2, :] > settings.hpi).any() & (vs.prec_day[2:-2, 2:-2, :] > 0).any() & (((vs.swe[2:-2, 2:-2, vs.tau] > 0).any() | (vs.swe_top[2:-2, 2:-2, vs.tau] > 0).any()) & (vs.ta_day[2:-2, 2:-2, :] > settings.ta_fm).any())
-#     cond4 = (vs.prec_day[2:-2, 2:-2, :] <= settings.hpi).all() & (vs.prec_day[2:-2, 2:-2, :] > 0).any() & (((vs.swe[2:-2, 2:-2, vs.tau] > 0).any() | (vs.swe_top[2:-2, 2:-2, vs.tau] > 0).any()) & (vs.ta_day[2:-2, 2:-2, :] > settings.ta_fm).any())
-#     cond5 = (vs.prec_day[2:-2, 2:-2, :] <= 0).all() & (((vs.swe[2:-2, 2:-2, vs.tau] > 0).any() | (vs.swe_top[2:-2, 2:-2, vs.tau] > 0).any()) & (vs.ta_day[2:-2, 2:-2, :] > settings.ta_fm).any())
-#     # no event | snowfall - daily time steps
-#     if cond0 | cond00:
-#         vs.update(calc_prec_ta_daily(state))
-#         if (vs.time % (24 * 60 * 60) == 0):
-#             vs.dt_secs = 24 * 60 * 60
-#         else:
-#             vs.dt_secs = 60 * 60
-#     # rainfall/snow melt event - hourly time steps
-#     elif (cond2 | cond4 | cond5) & ~ cond1 & ~ cond3:
-#         vs.update(calc_prec_ta_hourly(state))
-#         vs.dt_secs = 60 * 60
-#     # heavy rainfall event - 10 minutes time steps
-#     elif (cond1 | cond3) & ~ cond2 & ~ cond4 & ~ cond5:
-#         vs.update(calc_prec_ta_10_minutes(state))
-#         vs.dt_secs = 10 * 60
-#
-#     # determine end of event
-#     if ((vs.prec[2:-2, 2:-2] > 0).any() | ((vs.swe[2:-2, 2:-2, vs.tau] > 0) | (vs.swe_top[2:-2, 2:-2, vs.tau] > 0)).any() & (vs.ta[2:-2, 2:-2] > settings.ta_fm)).any():
-#         vs.time_event0 = 0
-#     elif ((vs.prec[2:-2, 2:-2] <= 0) & (vs.ta[2:-2, 2:-2] > settings.ta_fm)).all() | ((vs.prec[2:-2, 2:-2] > 0) & (vs.ta[2:-2, 2:-2] <= settings.ta_fm)).all() | ((vs.swe[2:-2, 2:-2, vs.taum1] > 0).any() & (vs.swe[2:-2, 2:-2, vs.tau] <= 0).all()):
-#         vs.time_event0 = vs.time_event0 + vs.dt_secs
-#
-#     # increase time stepping at end of event if either full hour
-#     # | full day, respectively
-#     if vs.time_event0 <= settings.end_event & (vs.dt_secs == 10 * 60):
-#         vs.update(calc_ta_pet_10_minutes(state))
-#         vs.event_id = update(
-#             vs.event_id,
-#             at[vs.tau], vs.event_id_counter,
-#         )
-#         vs.dt = 1 / 6
-#         vs.itt_day = vs.itt_day + 1
-#     elif vs.time_event0 <= settings.end_event & (vs.dt_secs == 60 * 60):
-#         vs.update(calc_ta_pet_hourly(state))
-#         vs.event_id = update(
-#             vs.event_id,
-#             at[vs.tau], vs.event_id_counter,
-#         )
-#         vs.dt = 1
-#         vs.itt_day = vs.itt_day + 6
-#     elif vs.time_event0 <= settings.end_event & (vs.dt_secs == 24 * 60 * 60):
-#         vs.update(calc_ta_pet_daily(state))
-#         vs.dt = 24
-#         vs.itt_day = 0
-#     elif vs.time_event0 > settings.end_event & (vs.time % (60 * 60) != 0) & (vs.dt_secs == 10 * 60):
-#         vs.update(calc_ta_pet_10_minutes(state))
-#         vs.dt_secs = 10 * 60
-#         vs.dt = 1 / 6
-#         vs.itt_day = vs.itt_day + 1
-#         vs.event_id = update(
-#             vs.event_id,
-#             at[vs.tau], 0,
-#         )
-#     elif vs.time_event0 > settings.end_event & (vs.time % (60 * 60) == 0) & ((vs.dt_secs == 10 * 60) | (vs.dt_secs == 60 * 60)):
-#         vs.update(calc_ta_pet_hourly(state))
-#         vs.dt_secs = 60 * 60
-#         vs.dt = 1
-#         vs.itt_day = vs.itt_day + 6
-#         vs.event_id = update(
-#             vs.event_id,
-#             at[vs.tau], 0,
-#         )
-#     elif vs.time_event0 > settings.end_event & (vs.time % (24 * 60 * 60) == 0) & (vs.dt_secs == 24 * 60 * 60):
-#         vs.update(calc_ta_pet_daily(state))
-#         vs.dt_secs = 24 * 60 * 60
-#         vs.dt = 24
-#         vs.itt_day = 0
-#         vs.event_id = update(
-#             vs.event_id,
-#             at[vs.tau], 0,
-#         )
-#
-#     # set event id for next event
-#     if (vs.event_id[vs.taum1] > 0) & (vs.event_id[vs.tau] == 0):
-#         vs.event_id_counter = vs.event_id_counter + 1
-#
-#     # set residual PET
-#     vs.pet_res = update(vs.pet_res, at[2:-2, 2:-2], vs.pet[2:-2, 2:-2])
-#
-#
-# @roger_kernel
-# def calc_prec_ta_10_minutes(state):
-#     vs = state.variables
-#
-#     vs.prec = update(
-#         vs.prec,
-#         at[2:-2, 2:-2, vs.tau], vs.prec_day[2:-2, 2:-2, vs.itt_day],
-#     )
-#     vs.ta = update(
-#         vs.ta,
-#         at[2:-2, 2:-2, vs.tau], vs.ta_day[2:-2, 2:-2, vs.itt_day],
-#     )
-#
-#     return KernelOutput(ta=vs.ta,
-#                         prec=vs.prec,
-#                         )
-#
-#
-# @roger_kernel
-# def calc_prec_ta_hourly(state):
-#     vs = state.variables
-#     idx = allocate(state.dimensions, ("x", "y", 6*24))
-#     idx = update(
-#         idx,
-#         at[2:-2, 2:-2, :], npx.arange(0, 6*24)[npx.newaxis, npx.newaxis, :],
-#     )
-#
-#     vs.prec = update(
-#         vs.prec,
-#         at[2:-2, 2:-2, vs.tau], npx.sum(npx.where((idx[2:-2, 2:-2, :] >= vs.itt_day) & (idx[2:-2, 2:-2, :] < vs.itt_day+6), vs.prec_day[2:-2, 2:-2, :], 0), axis=-1),
-#     )
-#     vs.ta = update(
-#         vs.ta,
-#         at[2:-2, 2:-2, vs.tau], npx.nanmean(npx.where((idx[2:-2, 2:-2, :] >= vs.itt_day) & (idx[2:-2, 2:-2, :] < vs.itt_day+6), vs.ta_day[2:-2, 2:-2, :], npx.nan), axis=-1),
-#     )
-#
-#     return KernelOutput(ta=vs.ta,
-#                         prec=vs.prec,
-#                         )
-#
-#
-# @roger_kernel
-# def calc_prec_ta_daily(state):
-#     vs = state.variables
-#
-#     vs.prec = update(
-#         vs.prec,
-#         at[2:-2, 2:-2, vs.tau], npx.sum(vs.prec_day, axis=-1)[2:-2, 2:-2],
-#     )
-#     vs.ta = update(
-#         vs.ta,
-#         at[2:-2, 2:-2, vs.tau], npx.mean(vs.ta_day[2:-2, 2:-2, 0:24*6], axis=-1),
-#     )
-#
-#     return KernelOutput(ta=vs.ta,
-#                         prec=vs.prec,
-#                         )
-#
-#
-# @roger_kernel
-# def calc_ta_pet_10_minutes(state):
-#     vs = state.variables
-#
-#     vs.ta = update(
-#         vs.ta,
-#         at[2:-2, 2:-2, vs.tau], vs.ta_day[2:-2, 2:-2, vs.itt_day],
-#     )
-#     vs.pet = update(
-#         vs.pet,
-#         at[2:-2, 2:-2], vs.pet_day[2:-2, 2:-2, vs.itt_day],
-#     )
-#
-#     return KernelOutput(ta=vs.ta,
-#                         pet=vs.pet,
-#                         )
-#
-#
-# @roger_kernel
-# def calc_ta_pet_hourly(state):
-#     vs = state.variables
-#
-#     idx = allocate(state.dimensions, ("x", "y", 6 * 24))
-#     idx = update(
-#         idx,
-#         at[2:-2, 2:-2, :], npx.arange(0, 6*24)[npx.newaxis, npx.newaxis, :],
-#     )
-#
-#     vs.ta = update(
-#         vs.ta,
-#         at[2:-2, 2:-2, vs.tau], npx.nanmean(npx.where((idx[2:-2, 2:-2, :] >= vs.itt_day) & (idx[2:-2, 2:-2, :] < vs.itt_day+6), vs.ta_day[2:-2, 2:-2, :], npx.nan), axis=-1),
-#     )
-#     vs.pet = update(
-#         vs.pet,
-#         at[2:-2, 2:-2], npx.sum(npx.where((idx[2:-2, 2:-2, :] >= vs.itt_day) & (idx[2:-2, 2:-2, :] < vs.itt_day+6), vs.pet_day[2:-2, 2:-2, :], 0), axis=-1),
-#     )
-#
-#     return KernelOutput(ta=vs.ta,
-#                         pet=vs.pet,
-#                         )
-#
-#
-# @roger_kernel
-# def calc_ta_pet_daily(state):
-#     vs = state.variables
-#
-#     vs.ta = update(
-#         vs.ta,
-#         at[2:-2, 2:-2, vs.tau], npx.mean(vs.ta_day[2:-2, 2:-2, 0:24*6], axis=-1),
-#     )
-#     vs.pet = update(
-#         vs.pet,
-#         at[2:-2, 2:-2], npx.sum(vs.pet_day[2:-2, 2:-2, 0:24*6], axis=-1),
-#     )
-#
-#     return KernelOutput(ta=vs.ta,
-#                         pet=vs.pet,
-#                         )
-
-
 @roger_routine
 def adaptive_time_stepping(state):
     vs = state.variables
 
     vs.update(adaptive_time_stepping_kernel(state))
```

### Comparing `roger-3.0/roger/core/capillary_rise.py` & `roger-3.0.1/roger/core/capillary_rise.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/crop.py` & `roger-3.0.1/roger/core/crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -771,18 +771,74 @@
         at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.z_root_crop[2:-2, 2:-2, vs.tau, :], vs.z_evap[2:-2, 2:-2, npx.newaxis])
     )
     vs.z_root = update(
         vs.z_root,
         at[2:-2, 2:-2, vs.tau], npx.where(npx.any(vs.crop_type[2:-2, 2:-2, :] == 598, axis=-1), vs.z_root[2:-2, 2:-2, vs.tau], npx.nanmax(z_root_crop[2:-2, 2:-2, :], axis=-1))
     )
 
+    # set thickness of upper soil water storage to 20 cm for bare soils
+    vs.z_root = update(
+        vs.z_root,
+        at[2:-2, 2:-2, vs.tau], npx.where(vs.z_root[2:-2, 2:-2, vs.tau] < 200, 200, vs.z_root[2:-2, 2:-2, vs.tau])
+    )
+    vs.z_root = update(
+        vs.z_root,
+        at[2:-2, 2:-2, vs.tau], npx.where(vs.z_root[2:-2, 2:-2, vs.tau] < vs.z_soil[2:-2, 2:-2], vs.z_root[2:-2, 2:-2, vs.tau], vs.z_soil[2:-2, 2:-2] * 0.9)
+    )
+
     return KernelOutput(z_root=vs.z_root)
 
 
 @roger_kernel
+def redistribution_pwp(state):
+    """
+    Calculates redistribution between root zone and subsoil after
+    root growth/root loss for immobile soil water storage (i.e. soil water below permanent wilting point)
+    """
+    vs = state.variables
+
+    uplift_root_growth_pwp = allocate(state.dimensions, ("x", "y"))
+    drain_root_loss_pwp = allocate(state.dimensions, ("x", "y"))
+
+    mask_root_growth = (vs.z_root[:, :, vs.tau] > vs.z_root[:, :, vs.taum1])
+    mask_root_loss = (vs.z_root[:, :, vs.tau] < vs.z_root[:, :, vs.taum1])
+
+    uplift_root_growth_pwp = update(
+        uplift_root_growth_pwp,
+        at[2:-2, 2:-2], (vs.z_root[2:-2, 2:-2, vs.tau] - vs.z_root[2:-2, 2:-2, vs.taum1]) * vs.theta_pwp[2:-2, 2:-2] * mask_root_growth[2:-2, 2:-2]
+    )
+    uplift_root_growth_pwp = update(
+        uplift_root_growth_pwp,
+        at[2:-2, 2:-2], npx.where(uplift_root_growth_pwp[2:-2, 2:-2] <= 0, 0, uplift_root_growth_pwp[2:-2, 2:-2])
+    )
+    drain_root_loss_pwp = update(
+        drain_root_loss_pwp,
+        at[2:-2, 2:-2], npx.abs(vs.z_root[2:-2, 2:-2, vs.taum1] - vs.z_root[2:-2, 2:-2, vs.tau]) * vs.theta_pwp[2:-2, 2:-2] * mask_root_loss[2:-2, 2:-2]
+    )
+    drain_root_loss_pwp = update(
+        drain_root_loss_pwp,
+        at[2:-2, 2:-2], npx.where(drain_root_loss_pwp[2:-2, 2:-2] <= 0, 0, drain_root_loss_pwp[2:-2, 2:-2])
+    )
+
+    # add redistribution of immobile soil water storage (i.e. soil water below permanent wilting point)
+    vs.re_rg_pwp = update(
+        vs.re_rg_pwp,
+        at[2:-2, 2:-2], npx.where(mask_root_growth[2:-2, 2:-2], uplift_root_growth_pwp[2:-2, 2:-2], 0)
+    )
+    vs.re_rl_pwp = update(
+        vs.re_rl_pwp,
+        at[2:-2, 2:-2], npx.where(mask_root_loss[2:-2, 2:-2], drain_root_loss_pwp[2:-2, 2:-2], 0)
+    )
+
+    return KernelOutput(
+        re_rg_pwp=vs.re_rg_pwp,
+        re_rl_pwp=vs.re_rl_pwp,
+        )
+
+@roger_kernel
 def redistribution(state):
     """
     Calculates redistribution between root zone and subsoil after
     root growth/root loss.
     """
     vs = state.variables
 
@@ -792,110 +848,119 @@
     drain_root_loss_fp = allocate(state.dimensions, ("x", "y"))
 
     mask_root_growth = (vs.z_root[:, :, vs.tau] > vs.z_root[:, :, vs.taum1])
     mask_root_loss = (vs.z_root[:, :, vs.tau] < vs.z_root[:, :, vs.taum1])
 
     uplift_root_growth_lp = update(
         uplift_root_growth_lp,
-        at[2:-2, 2:-2], ((vs.z_root[2:-2, 2:-2, vs.tau] - vs.z_root[2:-2, 2:-2, vs.taum1]) / (vs.z_soil[2:-2, 2:-2] - vs.z_root[2:-2, 2:-2, vs.taum1])) * vs.S_lp_ss[2:-2, 2:-2] * mask_root_growth[2:-2, 2:-2]
+        at[2:-2, 2:-2], npx.where(mask_root_growth[2:-2, 2:-2], ((vs.z_root[2:-2, 2:-2, vs.tau] - vs.z_root[2:-2, 2:-2, vs.taum1]) / (vs.z_soil[2:-2, 2:-2] - vs.z_root[2:-2, 2:-2, vs.taum1])) * vs.S_lp_ss[2:-2, 2:-2], 0)
     )
     uplift_root_growth_fp = update(
         uplift_root_growth_fp,
-        at[2:-2, 2:-2], ((vs.z_root[2:-2, 2:-2, vs.tau] - vs.z_root[2:-2, 2:-2, vs.taum1]) / (vs.z_soil[2:-2, 2:-2] - vs.z_root[2:-2, 2:-2, vs.taum1])) * vs.S_fp_ss[2:-2, 2:-2] * mask_root_growth[2:-2, 2:-2]
+        at[2:-2, 2:-2], npx.where(mask_root_growth[2:-2, 2:-2], ((vs.z_root[2:-2, 2:-2, vs.tau] - vs.z_root[2:-2, 2:-2, vs.taum1]) / (vs.z_soil[2:-2, 2:-2] - vs.z_root[2:-2, 2:-2, vs.taum1])) * vs.S_fp_ss[2:-2, 2:-2], 0)
     )
     uplift_root_growth_lp = update(
         uplift_root_growth_lp,
         at[2:-2, 2:-2], npx.where(uplift_root_growth_lp[2:-2, 2:-2] <= 0, 0, uplift_root_growth_lp[2:-2, 2:-2])
     )
     uplift_root_growth_fp = update(
         uplift_root_growth_fp,
         at[2:-2, 2:-2], npx.where(uplift_root_growth_fp[2:-2, 2:-2] <= 0, 0, uplift_root_growth_fp[2:-2, 2:-2])
     )
 
     drain_root_loss_lp = update(
         drain_root_loss_lp,
-        at[2:-2, 2:-2], ((vs.z_root[2:-2, 2:-2, vs.taum1] - vs.z_root[2:-2, 2:-2, vs.tau]) / vs.z_root[2:-2, 2:-2, vs.taum1]) * vs.S_lp_rz[2:-2, 2:-2] * mask_root_loss[2:-2, 2:-2]
+        at[2:-2, 2:-2], npx.where(mask_root_loss[2:-2, 2:-2], ((vs.z_root[2:-2, 2:-2, vs.taum1] - vs.z_root[2:-2, 2:-2, vs.tau]) / vs.z_root[2:-2, 2:-2, vs.taum1]) * vs.S_lp_rz[2:-2, 2:-2], 0)
     )
     drain_root_loss_fp = update(
         drain_root_loss_fp,
-        at[2:-2, 2:-2], ((vs.z_root[2:-2, 2:-2, vs.taum1] - vs.z_root[2:-2, 2:-2, vs.tau]) / vs.z_root[2:-2, 2:-2, vs.taum1]) * vs.S_fp_rz[2:-2, 2:-2] * mask_root_loss[2:-2, 2:-2]
+        at[2:-2, 2:-2], npx.where(mask_root_loss[2:-2, 2:-2], ((vs.z_root[2:-2, 2:-2, vs.taum1] - vs.z_root[2:-2, 2:-2, vs.tau]) / vs.z_root[2:-2, 2:-2, vs.taum1]) * vs.S_fp_rz[2:-2, 2:-2], 0)
     )
     drain_root_loss_lp = update(
         drain_root_loss_lp,
         at[2:-2, 2:-2], npx.where(drain_root_loss_lp[2:-2, 2:-2] <= 0, 0, drain_root_loss_lp[2:-2, 2:-2])
     )
     drain_root_loss_fp = update(
         drain_root_loss_fp,
         at[2:-2, 2:-2], npx.where(drain_root_loss_fp[2:-2, 2:-2] <= 0, 0, drain_root_loss_fp[2:-2, 2:-2])
     )
 
     vs.re_rg = update(
         vs.re_rg,
-        at[2:-2, 2:-2], (uplift_root_growth_fp[2:-2, 2:-2] + uplift_root_growth_lp[2:-2, 2:-2]) * mask_root_growth[2:-2, 2:-2]
+        at[2:-2, 2:-2], npx.where(mask_root_growth[2:-2, 2:-2], uplift_root_growth_fp[2:-2, 2:-2] + uplift_root_growth_lp[2:-2, 2:-2], 0)
     )
-
     vs.re_rl = update(
         vs.re_rl,
-        at[2:-2, 2:-2], (drain_root_loss_fp[2:-2, 2:-2] + drain_root_loss_lp[2:-2, 2:-2]) * mask_root_loss[2:-2, 2:-2]
+        at[2:-2, 2:-2], npx.where(mask_root_loss[2:-2, 2:-2], drain_root_loss_fp[2:-2, 2:-2] + drain_root_loss_lp[2:-2, 2:-2], 0)
     )
 
     # uplift from subsoil large pores
     vs.S_lp_ss = update_add(
         vs.S_lp_ss,
-        at[2:-2, 2:-2], - uplift_root_growth_lp[2:-2, 2:-2] * mask_root_growth[2:-2, 2:-2]
+        at[2:-2, 2:-2], npx.where(mask_root_growth[2:-2, 2:-2], -uplift_root_growth_lp[2:-2, 2:-2], 0)
     )
     # uplift from subsoil fine pores
     vs.S_fp_ss = update_add(
         vs.S_fp_ss,
-        at[2:-2, 2:-2], - uplift_root_growth_fp[2:-2, 2:-2] * mask_root_growth[2:-2, 2:-2]
+        at[2:-2, 2:-2], npx.where(mask_root_growth[2:-2, 2:-2], -uplift_root_growth_fp[2:-2, 2:-2], 0)
     )
 
     # update root zone storage
     vs.S_fp_rz = update_add(
         vs.S_fp_rz,
-        at[2:-2, 2:-2], vs.re_rg[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
+        at[2:-2, 2:-2], vs.re_rg[2:-2, 2:-2],
     )
 
     # fine pore excess fills large pores
     mask1 = (vs.S_fp_rz > vs.S_ufc_rz) & (vs.re_rg > 0)
     vs.S_lp_rz = update_add(
         vs.S_lp_rz,
-        at[2:-2, 2:-2], mask1[2:-2, 2:-2] * (vs.S_fp_rz[2:-2, 2:-2] - vs.S_ufc_rz[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+        at[2:-2, 2:-2], npx.where(mask1[2:-2, 2:-2], (vs.S_fp_rz[2:-2, 2:-2] - vs.S_ufc_rz[2:-2, 2:-2]), 0) * vs.maskCatch[2:-2, 2:-2],
     )
     vs.S_fp_rz = update(
         vs.S_fp_rz,
         at[2:-2, 2:-2], npx.where(mask1[2:-2, 2:-2], vs.S_ufc_rz[2:-2, 2:-2], vs.S_fp_rz[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
     )
 
     # drainage from root zone large pores
     vs.S_lp_rz = update_add(
         vs.S_lp_rz,
-        at[2:-2, 2:-2], - drain_root_loss_lp[2:-2, 2:-2] * mask_root_loss[2:-2, 2:-2],
+        at[2:-2, 2:-2], npx.where(mask_root_loss[2:-2, 2:-2], -drain_root_loss_lp[2:-2, 2:-2], 0),
     )
     # drainage from root zone fine pores
     vs.S_fp_rz = update_add(
         vs.S_fp_rz,
-        at[2:-2, 2:-2], - drain_root_loss_fp[2:-2, 2:-2] * mask_root_loss[2:-2, 2:-2],
+        at[2:-2, 2:-2], npx.where(mask_root_loss[2:-2, 2:-2], -drain_root_loss_fp[2:-2, 2:-2], 0),
     )
 
     # update subsoil storage
     vs.S_fp_ss = update_add(
         vs.S_fp_ss,
-        at[2:-2, 2:-2], vs.re_rl[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
+        at[2:-2, 2:-2], vs.re_rl[2:-2, 2:-2],
     )
 
-    # fine pore excess fills large pores
+    # fine pore excess storage fills large pores
     mask2 = (vs.S_fp_ss > vs.S_ufc_ss) & (vs.re_rl > 0)
     vs.S_lp_ss = update_add(
         vs.S_lp_ss,
-        at[2:-2, 2:-2], mask2[2:-2, 2:-2] * (vs.S_fp_ss[2:-2, 2:-2] - vs.S_ufc_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+        at[2:-2, 2:-2], npx.where(mask2[2:-2, 2:-2], (vs.S_fp_ss[2:-2, 2:-2] - vs.S_ufc_ss[2:-2, 2:-2]), 0),
     )
     vs.S_fp_ss = update(
         vs.S_fp_ss,
-        at[2:-2, 2:-2], npx.where(mask2[2:-2, 2:-2], vs.S_ufc_ss[2:-2, 2:-2], vs.S_fp_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+        at[2:-2, 2:-2], npx.where(mask2[2:-2, 2:-2], vs.S_ufc_ss[2:-2, 2:-2], vs.S_fp_ss[2:-2, 2:-2]),
+    )
+
+    # add redistribution of immobile soil water storage (i.e. soil water below permanent wilting point)
+    vs.re_rg = update_add(
+        vs.re_rg,
+        at[2:-2, 2:-2], npx.where( mask_root_growth[2:-2, 2:-2], vs.re_rg_pwp[2:-2, 2:-2], 0)
+    )
+    vs.re_rl = update_add(
+        vs.re_rl,
+        at[2:-2, 2:-2], npx.where(mask_root_loss[2:-2, 2:-2], vs.re_rl_pwp[2:-2, 2:-2], 0)
     )
 
     return KernelOutput(
         re_rg=vs.re_rg,
         re_rl=vs.re_rl,
         S_fp_rz=vs.S_fp_rz,
         S_lp_rz=vs.S_lp_rz,
@@ -1019,27 +1084,27 @@
         )
         vs.crop_height_max = update(
             vs.crop_height_max,
             at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.lut_crops[row_no, 16] * 1000, vs.crop_height_max[2:-2, 2:-2, :]),
         )
         vs.ccc_growth_rate = update(
             vs.ccc_growth_rate,
-            at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.lut_crops[row_no, 18], vs.ccc_growth_rate[2:-2, 2:-2, :]),
+            at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.lut_crops[row_no, 18] * vs.canopy_growth_scale[2:-2, 2:-2, npx.newaxis], vs.ccc_growth_rate[2:-2, 2:-2, :]),
         )
         vs.basal_crop_coeff_mid = update(
             vs.basal_crop_coeff_mid,
             at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.lut_crops[row_no, 21] * vs.lut_crop_scale[2:-2, 2:-2, row_no], vs.basal_crop_coeff_mid[2:-2, 2:-2, :]),
         )
         vs.z_root_crop_max = update(
             vs.z_root_crop_max,
             at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.lut_crops[row_no, 15] * 1000, vs.z_root_crop_max[2:-2, 2:-2, :]),
         )
         vs.root_growth_rate = update(
             vs.root_growth_rate,
-            at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.lut_crops[row_no, 19], vs.root_growth_rate[2:-2, 2:-2, :]),
+            at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.lut_crops[row_no, 19] * vs.root_growth_scale[2:-2, 2:-2, npx.newaxis], vs.root_growth_rate[2:-2, 2:-2, :]),
         )
         vs.water_stress_coeff_crop = update(
             vs.water_stress_coeff_crop,
             at[2:-2, 2:-2, :], npx.where(mask[2:-2, 2:-2, :], vs.lut_crops[row_no, 20], vs.water_stress_coeff_crop[2:-2, 2:-2, :]),
         )
 
     vs.theta_water_stress_crop = update(
@@ -1184,17 +1249,17 @@
             vs.update(update_ground_cover(state))
             vs.update(update_k_stress_transp(state))
             vs.update(update_basal_transp_coeff(state))
             vs.update(update_basal_evap_coeff(state))
             vs.update(update_S_int_ground_tot(state))
             vs.update(update_z_root(state))
             vs.update(recalc_soil_params(state))
+            vs.update(redistribution_pwp(state))
             vs.update(redistribution(state))
 
-
 @roger_kernel
 def update_alpha_transp(state):
     """
     Updates crop specific partition coefficient of transpiration
     """
     vs = state.variables
 
@@ -1340,24 +1405,29 @@
     )
 
     vs.TT_re_rg = update(
         vs.TT_re_rg,
         at[2:-2, 2:-2, 1:], npx.cumsum(vs.tt_re_rg[2:-2, 2:-2, :], axis=2),
     )
 
-    # calculate isotope travel time distribution
+    # calculate anion travel time distribution
     alpha = allocate(state.dimensions, ("x", "y"), fill=1)
     vs.mtt_re_rg = update(
         vs.mtt_re_rg,
         at[2:-2, 2:-2, :], transport.calc_mtt(state, vs.sa_ss, vs.tt_re_rg, vs.re_rg, vs.msa_ss, alpha)[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
     )
 
     vs.C_re_rg = update(
         vs.C_re_rg,
-        at[2:-2, 2:-2], npx.where(vs.re_rg > 0, npx.sum(vs.mtt_re_rg, axis=2) / vs.re_rg, 0)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
+        at[2:-2, 2:-2], npx.where(vs.re_rg[2:-2, 2:-2] > 0, npx.sum(vs.mtt_re_rg[2:-2, 2:-2, :], axis=-1) / vs.re_rg[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
+    )
+
+    vs.M_re_rg = update(
+        vs.M_re_rg,
+        at[2:-2, 2:-2], npx.sum(vs.mtt_re_rg[2:-2, 2:-2, :], axis=-1) * vs.maskCatch[2:-2, 2:-2],
     )
 
     # update StorAge with flux
     vs.sa_ss = update(
         vs.sa_ss,
         at[2:-2, 2:-2, :, :], transport.update_sa(state, vs.sa_ss, vs.tt_re_rg, vs.re_rg)[2:-2, 2:-2, :, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis, npx.newaxis],
     )
@@ -1374,15 +1444,15 @@
     )
     # update solute StorAge of subsoil
     vs.msa_ss = update_add(
         vs.msa_ss,
         at[2:-2, 2:-2, vs.tau, :], -vs.mtt_re_rg[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
     )
 
-    return KernelOutput(sa_rz=vs.sa_rz, sa_ss=vs.sa_ss, tt_re_rg=vs.tt_re_rg, TT_re_rg=vs.TT_re_rg, msa_rz=vs.msa_rz, msa_ss=vs.msa_ss, mtt_re_rg=vs.mtt_re_rg, C_re_rg=vs.C_re_rg, re_rg=vs.re_rg)
+    return KernelOutput(sa_rz=vs.sa_rz, sa_ss=vs.sa_ss, tt_re_rg=vs.tt_re_rg, TT_re_rg=vs.TT_re_rg, msa_rz=vs.msa_rz, msa_ss=vs.msa_ss, mtt_re_rg=vs.mtt_re_rg, M_re_rg=vs.M_re_rg, re_rg=vs.re_rg)
 
 
 @roger_kernel
 def calc_redistribution_root_loss_transport_kernel(state):
     """
     Calculates transport of redistribution after root loss
     """
@@ -1512,24 +1582,29 @@
     )
 
     vs.TT_re_rl = update(
         vs.TT_re_rl,
         at[2:-2, 2:-2, 1:], npx.cumsum(vs.tt_re_rl[2:-2, 2:-2, :], axis=2),
     )
 
-    # calculate isotope travel time distribution
+    # calculate anion travel time distribution
     alpha = allocate(state.dimensions, ("x", "y"), fill=1)
     vs.mtt_re_rl = update(
         vs.mtt_re_rl,
         at[2:-2, 2:-2, :], transport.calc_mtt(state, vs.sa_rz, vs.tt_re_rl, vs.re_rl, vs.msa_rz, alpha)[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
     )
 
     vs.C_re_rl = update(
         vs.C_re_rl,
-        at[2:-2, 2:-2], npx.where(vs.re_rg > 0, npx.sum(vs.mtt_re_rl, axis=2) / vs.re_rg, 0)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
+        at[2:-2, 2:-2], npx.where(vs.re_rl[2:-2, 2:-2] > 0, npx.sum(vs.mtt_re_rl[2:-2, 2:-2, :], axis=-1) / vs.re_rl[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
+    )
+
+    vs.M_re_rl = update(
+        vs.M_re_rl,
+        at[2:-2, 2:-2], npx.sum(vs.mtt_re_rl[2:-2, 2:-2, :], axis=-1) * vs.maskCatch[2:-2, 2:-2],
     )
 
     # update StorAge with flux
     vs.sa_rz = update(
         vs.sa_rz,
         at[2:-2, 2:-2, :, :], transport.update_sa(state, vs.sa_rz, vs.tt_re_rl, vs.re_rl)[2:-2, 2:-2, :, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis, npx.newaxis],
     )
@@ -1545,15 +1620,15 @@
     )
     # update solute StorAge of subsoil
     vs.msa_ss = update_add(
         vs.msa_ss,
         at[2:-2, 2:-2, vs.tau, :], vs.mtt_re_rl[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
     )
 
-    return KernelOutput(sa_rz=vs.sa_rz, sa_ss=vs.sa_ss, tt_re_rl=vs.tt_re_rl, TT_re_rl=vs.TT_re_rl, msa_rz=vs.msa_rz, msa_ss=vs.msa_ss, mtt_re_rl=vs.mtt_re_rl, C_re_rl=vs.C_re_rl, re_rl=vs.re_rl)
+    return KernelOutput(sa_rz=vs.sa_rz, sa_ss=vs.sa_ss, tt_re_rl=vs.tt_re_rl, TT_re_rl=vs.TT_re_rl, msa_rz=vs.msa_rz, msa_ss=vs.msa_ss, mtt_re_rl=vs.mtt_re_rl, C_re_rl=vs.C_re_rl, M_re_rl=vs.M_re_rl, re_rl=vs.re_rl)
 
 
 @roger_routine
 def calculate_redistribution_transport(state):
     """
     Calculates trasnport of redistribution after root growth/root loss
     """
```

### Comparing `roger-3.0/roger/core/evapotranspiration.py` & `roger-3.0.1/roger/core/evapotranspiration.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,15 +494,15 @@
         vs.msa_rz,
         at[2:-2, 2:-2, vs.tau, :], npx.where(vs.sa_rz[2:-2, 2:-2, vs.tau, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, vs.tau, :]) * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
     )
     return KernelOutput(sa_rz=vs.sa_rz, tt_evap_soil=vs.tt_evap_soil, TT_evap_soil=vs.TT_evap_soil, msa_rz=vs.msa_rz, mtt_evap_soil=vs.mtt_evap_soil, C_evap_soil=vs.C_evap_soil, C_iso_evap_soil=vs.C_iso_evap_soil)
 
 
 @roger_kernel
-def calculate_evaporation_transport_anion_kernel(state):
+def calc_evaporation_transport_virtualtracer_kernel(state):
     """
     Calculates transport of soil evaporation
     """
     vs = state.variables
     settings = state.settings
 
     vs.SA_rz = update(
@@ -516,43 +516,41 @@
     )
 
     vs.TT_evap_soil = update(
         vs.TT_evap_soil,
         at[2:-2, 2:-2, 1:], npx.cumsum(vs.tt_evap_soil[2:-2, 2:-2, :], axis=-1),
     )
 
-    if settings.enable_virtualtracer:
-        # calculate solute travel time distribution
-        alpha = allocate(state.dimensions, ("x", "y"), fill=1)
-        vs.mtt_evap_soil = update(
-            vs.mtt_evap_soil,
-            at[2:-2, 2:-2, :], transport.calc_mtt(state, vs.sa_rz, vs.tt_evap_soil, vs.evap_soil, vs.msa_rz, alpha)[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-        )
-        vs.C_evap_soil = update(
-            vs.C_evap_soil,
-            at[2:-2, 2:-2], npx.where(vs.evap_soil > 0, npx.sum(vs.mtt_evap_soil, axis=2) / vs.evap_soil, 0)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
-        )
-        vs.M_evap_soil = update(
-            vs.M_evap_soil,
-            at[2:-2, 2:-2], npx.sum(vs.mtt_evap_soil[2:-2, 2:-2, :], axis=-1) * vs.maskCatch[2:-2, 2:-2],
-        )
+    # calculate solute travel time distribution
+    alpha = allocate(state.dimensions, ("x", "y"), fill=1)
+    vs.mtt_evap_soil = update(
+        vs.mtt_evap_soil,
+        at[2:-2, 2:-2, :], transport.calc_mtt(state, vs.sa_rz, vs.tt_evap_soil, vs.evap_soil, vs.msa_rz, alpha)[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
+    )
+    vs.C_evap_soil = update(
+        vs.C_evap_soil,
+        at[2:-2, 2:-2], npx.where(vs.evap_soil > 0, npx.sum(vs.mtt_evap_soil, axis=2) / vs.evap_soil, 0)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
+    )
+    vs.M_evap_soil = update(
+        vs.M_evap_soil,
+        at[2:-2, 2:-2], npx.sum(vs.mtt_evap_soil[2:-2, 2:-2, :], axis=-1) * vs.maskCatch[2:-2, 2:-2],
+    )
 
     vs.sa_rz = update(
         vs.sa_rz,
         at[2:-2, 2:-2, :, :], transport.update_sa(state, vs.sa_rz, vs.tt_evap_soil, vs.evap_soil)[2:-2, 2:-2, :, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis, npx.newaxis],
     )
 
-    if settings.enable_virtualtracer:
-        # update solute StorAge of root zone
-        vs.msa_rz = update_add(
-            vs.msa_rz,
-            at[2:-2, 2:-2, vs.tau, :], - vs.mtt_evap_soil[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-        )
+    # update solute StorAge of root zone
+    vs.msa_rz = update_add(
+        vs.msa_rz,
+        at[2:-2, 2:-2, vs.tau, :], - vs.mtt_evap_soil[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
+    )
 
-    return KernelOutput(sa_rz=vs.sa_rz, tt_evap_soil=vs.tt_evap_soil, TT_evap_soil=vs.TT_evap_soil, msa_rz=vs.msa_rz, mtt_evap_soil=vs.mtt_evap_soil, C_evap_soil=vs.C_evap_soil, M_transp=vs.M_evap_soil)
+    return KernelOutput(sa_rz=vs.sa_rz, tt_evap_soil=vs.tt_evap_soil, TT_evap_soil=vs.TT_evap_soil, msa_rz=vs.msa_rz, mtt_evap_soil=vs.mtt_evap_soil, C_evap_soil=vs.C_evap_soil, M_evap_soil=vs.M_evap_soil)
 
 
 @roger_kernel
 def calc_transpiration_transport_kernel(state):
     """
     Calculates transport of transpiration
     """
@@ -696,10 +694,14 @@
         vs.update(calc_evaporation_transport_kernel(state))
         vs.update(calc_transpiration_transport_kernel(state))
 
     if settings.enable_offline_transport and (settings.enable_oxygen18 | settings.enable_deuterium):
         vs.update(calc_evaporation_transport_iso_kernel(state))
         vs.update(calc_transpiration_transport_iso_kernel(state))
 
-    if settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_nitrate | settings.enable_virtualtracer):
+    if settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_nitrate):
         vs.update(calc_evaporation_transport_kernel(state))
         vs.update(calc_transpiration_transport_anion_kernel(state))
+
+    if settings.enable_offline_transport and settings.enable_virtualtracer:
+        vs.update(calc_evaporation_transport_virtualtracer_kernel(state))
+        vs.update(calc_transpiration_transport_anion_kernel(state))
```

### Comparing `roger-3.0/roger/core/film_flow.py` & `roger-3.0.1/roger/core/film_flow.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/groundwater.py` & `roger-3.0.1/roger/core/groundwater.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/groundwater_flow.py` & `roger-3.0.1/roger/core/groundwater_flow.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/infiltration.py` & `roger-3.0.1/roger/core/infiltration.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/interception.py` & `roger-3.0.1/roger/core/interception.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/nitrate.py` & `roger-3.0.1/roger/core/nitrate.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/numerics.py` & `roger-3.0.1/roger/core/numerics.py`

 * *Files 20% similar despite different names*

```diff
@@ -175,55 +175,151 @@
             at[2:-2, 2:-2],
             npx.abs((vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1]) - (vs.prec[2:-2, 2:-2, vs.tau] - vs.q_sur[2:-2, 2:-2] - vs.aet[2:-2, 2:-2] - vs.q_ss[2:-2, 2:-2] - vs.q_sub[2:-2, 2:-2] + vs.cpr_ss[2:-2, 2:-2]))
             )
 
     elif settings.enable_lateral_flow and settings.enable_groundwater and not settings.enable_offline_transport:
         pass
 
-    elif not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and not settings.enable_groundwater and not settings.enable_offline_transport:
+    elif not settings.enable_crop_phenology and not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and not settings.enable_groundwater and not settings.enable_offline_transport:
         vs.dS_num_error = update(
             vs.dS_num_error,
             at[2:-2, 2:-2],
             npx.abs((vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1]) - (vs.prec[2:-2, 2:-2, vs.tau] - vs.q_sur[2:-2, 2:-2] - vs.aet[2:-2, 2:-2] - vs.q_ss[2:-2, 2:-2]))
             )
-
+        
+        vs.dS_rz_num_error = update(
+            vs.dS_rz_num_error,
+            at[2:-2, 2:-2],
+            npx.abs((vs.S_rz[2:-2, 2:-2, vs.tau] - vs.S_rz[2:-2, 2:-2, vs.taum1]) - (vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_mp_rz[2:-2, 2:-2] + vs.inf_sc_rz[2:-2, 2:-2] + vs.cpr_rz[2:-2, 2:-2] - vs.transp[2:-2, 2:-2] - vs.evap_soil[2:-2, 2:-2] - vs.q_rz[2:-2, 2:-2]))
+            )
+        
+        vs.dS_ss_num_error = update(
+            vs.dS_ss_num_error,
+            at[2:-2, 2:-2],
+            npx.abs((vs.S_ss[2:-2, 2:-2, vs.tau] - vs.S_ss[2:-2, 2:-2, vs.taum1]) - (vs.inf_mp_ss[2:-2, 2:-2] + vs.q_rz[2:-2, 2:-2] - vs.q_ss[2:-2, 2:-2] - vs.cpr_rz[2:-2, 2:-2]))
+            )
+                
+    elif settings.enable_crop_phenology and not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and not settings.enable_groundwater and not settings.enable_offline_transport:
+        vs.dS_num_error = update(
+            vs.dS_num_error,
+            at[2:-2, 2:-2],
+            npx.abs((vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1]) - (vs.prec[2:-2, 2:-2, vs.tau] - vs.q_sur[2:-2, 2:-2] - vs.aet[2:-2, 2:-2] - vs.q_ss[2:-2, 2:-2]))
+            )
+        
+        vs.dS_rz_num_error = update(
+            vs.dS_rz_num_error,
+            at[2:-2, 2:-2],
+            npx.abs((vs.S_rz[2:-2, 2:-2, vs.tau] - vs.S_rz[2:-2, 2:-2, vs.taum1]) - (vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_mp_rz[2:-2, 2:-2] + vs.inf_sc_rz[2:-2, 2:-2] + vs.cpr_rz[2:-2, 2:-2] + vs.re_rg[2:-2, 2:-2] - vs.transp[2:-2, 2:-2] - vs.evap_soil[2:-2, 2:-2] - vs.q_rz[2:-2, 2:-2] - vs.re_rl[2:-2, 2:-2]))
+            )
+        
+        vs.dS_ss_num_error = update(
+            vs.dS_ss_num_error,
+            at[2:-2, 2:-2],
+            npx.abs((vs.S_ss[2:-2, 2:-2, vs.tau] - vs.S_ss[2:-2, 2:-2, vs.taum1]) - (vs.inf_mp_ss[2:-2, 2:-2] + vs.q_rz[2:-2, 2:-2] + vs.re_rl[2:-2, 2:-2] - vs.re_rg[2:-2, 2:-2] - vs.q_ss[2:-2, 2:-2] - vs.cpr_rz[2:-2, 2:-2]))
+            )
+        
     elif not settings.enable_lateral_flow and settings.enable_groundwater_boundary and not settings.enable_groundwater and not settings.enable_offline_transport:
         vs.dS_num_error = update(
             vs.dS_num_error,
             at[2:-2, 2:-2],
             npx.abs((vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1]) - (vs.prec[2:-2, 2:-2, vs.tau] - vs.q_sur[2:-2, 2:-2] - vs.aet[2:-2, 2:-2] - vs.q_ss[2:-2, 2:-2] + vs.cpr_ss[2:-2, 2:-2]))
             )
 
     elif settings.enable_offline_transport and not (settings.enable_groundwater_boundary | settings.enable_crop_phenology):
         vs.dS_num_error = update(
             vs.dS_num_error,
             at[2:-2, 2:-2], npx.abs((npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1)) - (vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] -
             npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2)) * settings.h)
         )
+    elif settings.enable_offline_transport and settings.enable_crop_phenology and not settings.enable_groundwater_boundary:
+        vs.dS_num_error = update(
+            vs.dS_num_error,
+            at[2:-2, 2:-2], npx.abs((npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1)) - (vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] -
+            npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2)) * settings.h)
+        )
     return KernelOutput(
         dS_num_error=vs.dS_num_error,
+        dS_rz_num_error=vs.dS_rz_num_error,
+        dS_ss_num_error=vs.dS_ss_num_error,
         )
 
 
 @roger_kernel
 def calc_dC_num_error(state):
     """
     Calculates numerical error of solute balance
     """
     vs = state.variables
     settings = state.settings
 
-    if settings.enable_offline_transport and not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and (settings.enable_deuterium or settings.enable_oxygen18 or settings.enable_bromide or settings.enable_chloride):
+    if settings.enable_offline_transport and not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and (settings.enable_deuterium or settings.enable_oxygen18):
         vs.dC_num_error = update(
             vs.dC_num_error,
             at[2:-2, 2:-2], npx.abs((npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.tau] - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.taum1]) - (vs.inf_mat_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_mat_rz[2:-2, 2:-2]), 0, vs.C_inf_mat_rz[2:-2, 2:-2]) + vs.inf_pf_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_rz[2:-2, 2:-2]), 0, vs.C_inf_pf_rz[2:-2, 2:-2]) + vs.inf_pf_ss[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_ss[2:-2, 2:-2]), 0, vs.C_inf_pf_ss[2:-2, 2:-2]) - npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_evap_soil[2:-2, 2:-2]), 0, vs.C_evap_soil[2:-2, 2:-2]) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_transp[2:-2, 2:-2]), 0, vs.C_transp[2:-2, 2:-2]) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_q_ss[2:-2, 2:-2]), 0, vs.C_q_ss[2:-2, 2:-2])) * settings.h)
         )
 
+    elif settings.enable_offline_transport and not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and settings.enable_virtualtracer:
+        vs.dC_num_error = update(
+            vs.dC_num_error,
+            at[2:-2, 2:-2], npx.abs((npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.tau] - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.taum1]) - (vs.inf_mat_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_mat_rz[2:-2, 2:-2]), 0, vs.C_inf_mat_rz[2:-2, 2:-2]) + vs.inf_pf_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_rz[2:-2, 2:-2]), 0, vs.C_inf_pf_rz[2:-2, 2:-2]) + vs.inf_pf_ss[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_ss[2:-2, 2:-2]), 0, vs.C_inf_pf_ss[2:-2, 2:-2]) - npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_evap_soil[2:-2, 2:-2]), 0, vs.C_evap_soil[2:-2, 2:-2]) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_transp[2:-2, 2:-2]), 0, vs.C_transp[2:-2, 2:-2]) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_q_ss[2:-2, 2:-2]), 0, vs.C_q_ss[2:-2, 2:-2])) * settings.h)
+        )
+
+    elif settings.enable_offline_transport and settings.enable_crop_phenology and not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and settings.enable_virtualtracer:
+        vs.dC_num_error = update(
+            vs.dC_num_error,
+            at[2:-2, 2:-2], npx.abs((npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.tau] - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.taum1]) - (vs.inf_mat_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_mat_rz[2:-2, 2:-2]), 0, vs.C_inf_mat_rz[2:-2, 2:-2]) + vs.inf_pf_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_rz[2:-2, 2:-2]), 0, vs.C_inf_pf_rz[2:-2, 2:-2]) + vs.inf_pf_ss[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_ss[2:-2, 2:-2]), 0, vs.C_inf_pf_ss[2:-2, 2:-2]) - npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_evap_soil[2:-2, 2:-2]), 0, vs.C_evap_soil[2:-2, 2:-2]) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_transp[2:-2, 2:-2]), 0, vs.C_transp[2:-2, 2:-2]) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_q_ss[2:-2, 2:-2]), 0, vs.C_q_ss[2:-2, 2:-2])) * settings.h)
+        )
+
+        vs.dC_rz_num_error = update(
+            vs.dC_rz_num_error,
+            at[2:-2, 2:-2], npx.abs((npx.sum(vs.sa_rz[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.C_rz[2:-2, 2:-2, vs.tau] - 
+                                     npx.sum(vs.sa_rz[2:-2, 2:-2, vs.taum1, :], axis=-1) * vs.C_rz[2:-2, 2:-2, vs.taum1]) - 
+                                     (vs.inf_mat_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_mat_rz[2:-2, 2:-2]), 0, vs.C_inf_mat_rz[2:-2, 2:-2]) + 
+                                      vs.inf_pf_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_rz[2:-2, 2:-2]), 0, vs.C_inf_pf_rz[2:-2, 2:-2]) + 
+                                      npx.sum(vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_cpr_rz[2:-2, 2:-2]), 0, vs.C_cpr_rz[2:-2, 2:-2]) +
+                                      npx.sum(vs.re_rg[2:-2, 2:-2, npx.newaxis] * vs.tt_re_rg[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_re_rg[2:-2, 2:-2]), 0, vs.C_re_rg[2:-2, 2:-2]) - 
+                                      npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_evap_soil[2:-2, 2:-2]), 0, vs.C_evap_soil[2:-2, 2:-2]) - 
+                                      npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_transp[2:-2, 2:-2]), 0, vs.C_transp[2:-2, 2:-2]) - 
+                                      npx.sum(vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_q_rz[2:-2, 2:-2]), 0, vs.C_q_rz[2:-2, 2:-2]) -
+                                      npx.sum(vs.re_rl[2:-2, 2:-2, npx.newaxis] * vs.tt_re_rl[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_re_rl[2:-2, 2:-2]), 0, vs.C_re_rl[2:-2, 2:-2])) * settings.h)
+        )
+
+        vs.dC_ss_num_error = update(
+            vs.dC_ss_num_error,
+            at[2:-2, 2:-2], npx.abs((npx.sum(vs.sa_ss[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.C_ss[2:-2, 2:-2, vs.tau] - 
+                                     npx.sum(vs.sa_ss[2:-2, 2:-2, vs.taum1, :], axis=-1) * vs.C_ss[2:-2, 2:-2, vs.taum1]) - 
+                                     (vs.inf_pf_ss[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_ss[2:-2, 2:-2]), 0, vs.C_inf_pf_ss[2:-2, 2:-2]) + 
+                                      npx.sum(vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_q_rz[2:-2, 2:-2]), 0, vs.C_q_rz[2:-2, 2:-2]) +
+                                      npx.sum(vs.re_rl[2:-2, 2:-2, npx.newaxis] * vs.tt_re_rl[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_re_rl[2:-2, 2:-2]), 0, vs.C_re_rl[2:-2, 2:-2]) - 
+                                      npx.sum(vs.re_rg[2:-2, 2:-2, npx.newaxis] * vs.tt_re_rg[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_re_rg[2:-2, 2:-2]), 0, vs.C_re_rg[2:-2, 2:-2]) -
+                                      npx.sum(vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_cpr_rz[2:-2, 2:-2]), 0, vs.C_cpr_rz[2:-2, 2:-2]) -
+                                      npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * 
+                                      npx.where(npx.isnan(vs.C_q_ss[2:-2, 2:-2]), 0, vs.C_q_ss[2:-2, 2:-2])) * settings.h)
+        )
+
+    elif settings.enable_offline_transport and not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and (settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate):
+        vs.dC_num_error = update(
+            vs.dC_num_error,
+            at[2:-2, 2:-2], npx.abs((npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.tau] - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.taum1]) - (vs.inf_mat_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_mat_rz[2:-2, 2:-2]), 0, vs.C_inf_mat_rz[2:-2, 2:-2]) + vs.inf_pf_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_rz[2:-2, 2:-2]), 0, vs.C_inf_pf_rz[2:-2, 2:-2]) + vs.inf_pf_ss[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_ss[2:-2, 2:-2]), 0, vs.C_inf_pf_ss[2:-2, 2:-2]) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_transp[2:-2, 2:-2]), 0, vs.C_transp[2:-2, 2:-2]) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_q_ss[2:-2, 2:-2]), 0, vs.C_q_ss[2:-2, 2:-2])) * settings.h)
+        )
+
     return KernelOutput(
         dC_num_error=vs.dC_num_error,
+        dC_rz_num_error=vs.dC_rz_num_error,
+        dC_ss_num_error=vs.dC_ss_num_error,
         )
 
 
 @roger_routine
 def calculate_num_error(state):
     vs = state.variables
     settings = state.settings
@@ -239,14 +335,16 @@
 def sanity_check(state):
     """
     Checks for mass conservation
     """
     vs = state.variables
     settings = state.settings
 
+    check = True
+
     if settings.enable_lateral_flow and not settings.enable_groundwater_boundary and not settings.enable_groundwater and not settings.enable_offline_transport:
         check1 = global_and(npx.all(npx.isclose(vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1], vs.prec[2:-2, 2:-2, vs.tau] - vs.q_sur[2:-2, 2:-2] - vs.aet[2:-2, 2:-2] - vs.q_ss[2:-2, 2:-2] - vs.q_sub[2:-2, 2:-2], atol=settings.atol, rtol=settings.rtol)))
         check2 = global_and(npx.all((vs.S_fp_rz[2:-2, 2:-2] > -settings.atol) & (vs.S_lp_rz[2:-2, 2:-2] > -settings.atol) & (vs.S_fp_ss[2:-2, 2:-2] > -settings.atol) & (vs.S_lp_ss[2:-2, 2:-2] > -settings.atol)))
         check3 = global_and(npx.all((vs.S_fp_rz[2:-2, 2:-2] - settings.atol <= vs.S_ufc_rz[2:-2, 2:-2]) & (vs.S_lp_rz[2:-2, 2:-2] - settings.atol <= vs.S_ac_rz[2:-2, 2:-2]) & (vs.S_fp_ss[2:-2, 2:-2] - settings.atol <= vs.S_ufc_ss[2:-2, 2:-2]) & (vs.S_lp_ss[2:-2, 2:-2] - settings.atol <= vs.S_ac_ss[2:-2, 2:-2])))
         check = check1 & check2 & check3
 
     elif settings.enable_lateral_flow and settings.enable_groundwater_boundary and not settings.enable_offline_transport:
@@ -275,20 +373,20 @@
 
     elif not settings.enable_lateral_flow and not settings.enable_groundwater_boundary and not settings.enable_groundwater and not settings.enable_offline_transport:
         check1 = global_and(npx.all(npx.isclose(vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1], vs.prec[2:-2, 2:-2, vs.tau] - vs.q_sur[2:-2, 2:-2] - vs.aet[2:-2, 2:-2] - vs.q_ss[2:-2, 2:-2], atol=settings.atol, rtol=settings.rtol)))
         check2 = global_and(npx.all((vs.S_fp_rz[2:-2, 2:-2] > -settings.atol) & (vs.S_lp_rz[2:-2, 2:-2] > -settings.atol) & (vs.S_fp_ss[2:-2, 2:-2] > -settings.atol) & (vs.S_lp_ss[2:-2, 2:-2] > -settings.atol)))
         check3 = global_and(npx.all((vs.S_fp_rz[2:-2, 2:-2] - settings.atol <= vs.S_ufc_rz[2:-2, 2:-2]) & (vs.S_lp_rz[2:-2, 2:-2] - settings.atol <= vs.S_ac_rz[2:-2, 2:-2]) & (vs.S_fp_ss[2:-2, 2:-2] - settings.atol <= vs.S_ufc_ss[2:-2, 2:-2]) & (vs.S_lp_ss[2:-2, 2:-2] - settings.atol <= vs.S_ac_ss[2:-2, 2:-2])))
         check = check1 & check2 & check3
 
-    elif settings.enable_offline_transport and not (settings.enable_deuterium or settings.enable_oxygen18 or settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate):
+    elif settings.enable_offline_transport and not settings.enable_groundwater_boundary and not (settings.enable_deuterium or settings.enable_oxygen18 or settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer):
         check = global_and(npx.all(npx.isclose(npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1),
                                                (vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] -
                                                npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2)) * settings.h, atol=settings.atol, rtol=settings.rtol)))
 
-    elif settings.enable_offline_transport and (settings.enable_deuterium or settings.enable_oxygen18):
+    elif settings.enable_offline_transport and not settings.enable_groundwater_boundary and (settings.enable_deuterium or settings.enable_oxygen18):
         check1 = global_and(npx.all(npx.isclose(npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1),
                                                 (vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] -
                                                 npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2)) * settings.h, atol=settings.atol, rtol=settings.rtol)))
         check2 = global_and(npx.all(npx.isclose(npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.tau] - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1) * vs.C_s[2:-2, 2:-2, vs.taum1],
                                                 (vs.inf_mat_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_mat_rz[2:-2, 2:-2]), 0, vs.C_inf_mat_rz[2:-2, 2:-2]) + vs.inf_pf_rz[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_rz[2:-2, 2:-2]), 0, vs.C_inf_pf_rz[2:-2, 2:-2]) + vs.inf_pf_ss[2:-2, 2:-2] * npx.where(npx.isnan(vs.C_inf_pf_ss[2:-2, 2:-2]), 0, vs.C_inf_pf_ss[2:-2, 2:-2]) -
                                                 npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_evap_soil[2:-2, 2:-2]), 0, vs.C_evap_soil[2:-2, 2:-2]) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_transp[2:-2, 2:-2]), 0, vs.C_transp[2:-2, 2:-2]) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * npx.where(npx.isnan(vs.C_q_ss[2:-2, 2:-2]), 0, vs.C_q_ss[2:-2, 2:-2])) * settings.h, atol=settings.atol, rtol=settings.rtol)))
         check = check1 & check2
@@ -342,25 +440,35 @@
                 logger.warning(f"Root zone StorAge is out of bounds at iteration {vs.itt}")
                 rows55 = npx.where(npx.any(check55 == False, axis=-1))[0].tolist()
                 cols55 = npx.where(npx.any(check55 == False, axis=-1))[1].tolist()
                 rowscols55 = tuple(zip(rows55, cols55))
                 if rowscols55:
                     logger.warning(f"Root zone StorAge is out of bounds at at {rowscols55}")
 
-    elif settings.enable_offline_transport and (settings.enable_bromide or settings.enable_chloride):
+    elif settings.enable_offline_transport and not settings.enable_groundwater_boundary and (settings.enable_bromide or settings.enable_chloride):
         check1 = global_and(npx.all(npx.isclose(npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1),
                                                 vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] -
                                                 npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2), atol=settings.atol, rtol=settings.rtol)))
         check2 = global_and(npx.all(npx.isclose(npx.sum(vs.msa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.msa_s[2:-2, 2:-2, vs.taum1, :], axis=-1),
                                                 vs.inf_mat_rz[2:-2, 2:-2] * vs.C_inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] * vs.C_inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] * vs.C_inf_pf_ss[2:-2, 2:-2] -
                                                 npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * vs.C_transp[2:-2, 2:-2] - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * vs.C_q_ss[2:-2, 2:-2], atol=settings.atol, rtol=settings.rtol)))
 
         check = check1 & check2
 
-    elif settings.enable_offline_transport and settings.enable_nitrate:
+    elif settings.enable_offline_transport and not settings.enable_groundwater_boundary and settings.enable_virtualtracer:
+        check1 = global_and(npx.all(npx.isclose(npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1),
+                                                vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] -
+                                                npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2), atol=settings.atol, rtol=settings.rtol)))
+        check2 = global_and(npx.all(npx.isclose(npx.sum(vs.msa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.msa_s[2:-2, 2:-2, vs.taum1, :], axis=-1),
+                                                vs.inf_mat_rz[2:-2, 2:-2] * vs.C_inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] * vs.C_inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] * vs.C_inf_pf_ss[2:-2, 2:-2] -
+                                                npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * vs.C_transp[2:-2, 2:-2] - npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) * vs.C_evap_soil[2:-2, 2:-2] - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * vs.C_q_ss[2:-2, 2:-2], atol=settings.atol, rtol=settings.rtol)))
+
+        check = check1 & check2
+
+    elif settings.enable_offline_transport and not settings.enable_groundwater_boundary and settings.enable_nitrate:
         check1 = global_and(npx.all(npx.isclose(npx.sum(vs.sa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.sa_s[2:-2, 2:-2, vs.taum1, :], axis=-1),
                                                 vs.inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] -
                                                 npx.sum(vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :], axis=2) - npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2), atol=settings.atol, rtol=settings.rtol)))
         check2 = global_and(npx.all(npx.isclose(npx.sum(vs.msa_s[2:-2, 2:-2, vs.tau, :], axis=-1) - npx.sum(vs.msa_s[2:-2, 2:-2, vs.taum1, :], axis=-1),
                                                 vs.inf_mat_rz[2:-2, 2:-2] * vs.C_inf_mat_rz[2:-2, 2:-2] + vs.inf_pf_rz[2:-2, 2:-2] * vs.C_inf_pf_rz[2:-2, 2:-2] + vs.inf_pf_ss[2:-2, 2:-2] * vs.C_inf_pf_ss[2:-2, 2:-2] + npx.sum(vs.ma_s[2:-2, 2:-2, :], axis=2) -
                                                 npx.sum(vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :], axis=2) * vs.C_transp[2:-2, 2:-2] - npx.sum(vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :], axis=2) * vs.C_q_ss[2:-2, 2:-2] - npx.sum(vs.mr_s[2:-2, 2:-2, :], axis=2), atol=settings.atol, rtol=settings.rtol)))
```

### Comparing `roger-3.0/roger/core/operators.py` & `roger-3.0.1/roger/core/operators.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/root_zone.py` & `roger-3.0.1/roger/core/root_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,29 +69,29 @@
 @roger_kernel
 def calc_S(state):
     """
     Calculates soil water content of root zone
     """
     vs = state.variables
 
-    # horizontal redistribution
-    mask = (vs.S_fp_rz < vs.S_ufc_rz) & (vs.S_fp_rz >= 0) & (vs.S_lp_rz < vs.S_ac_rz) & (vs.S_lp_rz > 0)
-    S_fp_rz = allocate(state.dimensions, ("x", "y"))
-    S_fp_rz = update(
-        S_fp_rz,
-        at[2:-2, 2:-2], vs.S_fp_rz[2:-2, 2:-2],
-    )
-    vs.S_fp_rz = update(
-        vs.S_fp_rz,
-        at[2:-2, 2:-2], npx.where(mask[2:-2, 2:-2], npx.where((vs.S_ufc_rz[2:-2, 2:-2] - vs.S_fp_rz[2:-2, 2:-2] > vs.S_lp_rz[2:-2, 2:-2]), vs.S_fp_rz[2:-2, 2:-2] + vs.S_lp_rz[2:-2, 2:-2], vs.S_ufc_rz[2:-2, 2:-2]), vs.S_fp_rz[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
-    )
-    vs.S_lp_rz = update(
-        vs.S_lp_rz,
-        at[2:-2, 2:-2], npx.where(mask[2:-2, 2:-2], npx.where((vs.S_ufc_rz[2:-2, 2:-2] - S_fp_rz[2:-2, 2:-2] > vs.S_lp_rz[2:-2, 2:-2]), 0, vs.S_lp_rz[2:-2, 2:-2] - (vs.S_ufc_rz[2:-2, 2:-2] - S_fp_rz[2:-2, 2:-2])), vs.S_lp_rz[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
-    )
+    # # horizontal redistribution
+    # mask = (vs.S_fp_rz < vs.S_ufc_rz) & (vs.S_fp_rz >= 0) & (vs.S_lp_rz < vs.S_ac_rz) & (vs.S_lp_rz > 0)
+    # S_fp_rz = allocate(state.dimensions, ("x", "y"))
+    # S_fp_rz = update(
+    #     S_fp_rz,
+    #     at[2:-2, 2:-2], vs.S_fp_rz[2:-2, 2:-2],
+    # )
+    # vs.S_fp_rz = update(
+    #     vs.S_fp_rz,
+    #     at[2:-2, 2:-2], npx.where(mask[2:-2, 2:-2], npx.where((vs.S_ufc_rz[2:-2, 2:-2] - vs.S_fp_rz[2:-2, 2:-2] > vs.S_lp_rz[2:-2, 2:-2]), vs.S_fp_rz[2:-2, 2:-2] + vs.S_lp_rz[2:-2, 2:-2], vs.S_ufc_rz[2:-2, 2:-2]), vs.S_fp_rz[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    # )
+    # vs.S_lp_rz = update(
+    #     vs.S_lp_rz,
+    #     at[2:-2, 2:-2], npx.where(mask[2:-2, 2:-2], npx.where((vs.S_ufc_rz[2:-2, 2:-2] - S_fp_rz[2:-2, 2:-2] > vs.S_lp_rz[2:-2, 2:-2]), 0, vs.S_lp_rz[2:-2, 2:-2] - (vs.S_ufc_rz[2:-2, 2:-2] - S_fp_rz[2:-2, 2:-2])), vs.S_lp_rz[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    # )
 
     vs.S_rz = update(
         vs.S_rz,
         at[2:-2, 2:-2, vs.tau], (vs.S_pwp_rz[2:-2, 2:-2] + vs.S_fp_rz[2:-2, 2:-2] + vs.S_lp_rz[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
     )
 
     return KernelOutput(S_rz=vs.S_rz)
```

### Comparing `roger-3.0/roger/core/sas.py` & `roger-3.0.1/roger/core/sas.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/snow.py` & `roger-3.0.1/roger/core/snow.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/soil.py` & `roger-3.0.1/roger/core/soil.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,19 @@
         vs.tew,
         at[2:-2, 2:-2], ((vs.theta_fc[2:-2, 2:-2] - 0.5 * vs.theta_pwp[2:-2, 2:-2]) * vs.z_evap[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2]
     )
 
     # root depth
     z_root = allocate(state.dimensions, ("x", "y"))
 
+    z_root = update(
+        z_root,
+        at[2:-2, 2:-2], vs.z_root[2:-2, 2:-2, 0]
+    )
+
     cc_cond = allocate(state.dimensions, ("x", "y"), dtype=bool, fill=False)
     cc_cond = update(
         cc_cond,
         at[:, :], npx.isin(vs.lu_id, npx.array([0, 5, 6, 7, 8, 9, 10, 11, 12, 13, 15, 98, 31, 32, 33, 40, 41, 50, 98]))
     )
 
     # assign land use specific root depth
@@ -339,32 +344,27 @@
     )
 
     z_root = update(
         z_root,
         at[2:-2, 2:-2], npx.where((z_root[2:-2, 2:-2] >= vs.z_soil[2:-2, 2:-2]), 0.9 * vs.z_soil[2:-2, 2:-2], z_root[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2]
     )
 
+    # set thickness of upper soil water storage to 20 cm for bare soils
+    mask_crops = npx.isin(vs.lu_id, npx.arange(500, 600, 1, dtype=npx.int64))
     vs.z_root = update(
         vs.z_root,
-        at[2:-2, 2:-2, 0], z_root[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2]
-    )
-
-    vs.z_root = update(
-        vs.z_root,
-        at[2:-2, 2:-2, 1], z_root[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2]
+        at[2:-2, 2:-2, 0], npx.where(mask_crops[2:-2, 2:-2], 200, vs.z_root[2:-2, 2:-2, 0]) * vs.maskCatch[2:-2, 2:-2]
     )
-
-    mask_crops = npx.isin(vs.lu_id, npx.arange(500, 600, 1, dtype=int))
     vs.z_root = update(
         vs.z_root,
-        at[2:-2, 2:-2, 0], npx.where(mask_crops[2:-2, 2:-2], vs.z_evap[2:-2, 2:-2], vs.z_root[2:-2, 2:-2, 0]) * vs.maskCatch[2:-2, 2:-2]
+        at[2:-2, 2:-2, 1], npx.where(mask_crops[2:-2, 2:-2], 200, vs.z_root[2:-2, 2:-2, 1]) * vs.maskCatch[2:-2, 2:-2]
     )
     vs.z_root = update(
         vs.z_root,
-        at[2:-2, 2:-2, 1], npx.where(mask_crops[2:-2, 2:-2], vs.z_evap[2:-2, 2:-2], vs.z_root[2:-2, 2:-2, 1]) * vs.maskCatch[2:-2, 2:-2]
+        at[2:-2, 2:-2, :], npx.where(vs.z_root[2:-2, 2:-2, :] < vs.z_soil[2:-2, 2:-2, npx.newaxis], vs.z_root[2:-2, 2:-2, :], vs.z_soil[2:-2, 2:-2, npx.newaxis] * 0.9)
     )
 
     vs.S_ac_rz = update(
         vs.S_ac_rz,
         at[2:-2, 2:-2], (vs.theta_ac[2:-2, 2:-2] * vs.z_root[2:-2, 2:-2, vs.tau]) * vs.maskCatch[2:-2, 2:-2]
     )
 
@@ -913,15 +913,15 @@
 
     if settings.enable_offline_transport and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate):
         vs.update(calculate_soil_transport_kernel(state))
 
     if settings.enable_offline_transport and (settings.enable_oxygen18 | settings.enable_deuterium):
         vs.update(calculate_soil_transport_iso_kernel(state))
 
-    if settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_nitrate):
+    if settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_nitrate | settings.enable_virtualtracer):
         vs.update(calculate_soil_transport_anion_kernel(state))
 
 
 @roger_kernel
 def rescale_sa_soil_kernel(state):
     """
     Rescale StorAge.
@@ -1177,15 +1177,15 @@
             at[2:-2, 2:-2, :2, 1:], npx.cumsum(vs.sa_s[2:-2, 2:-2, :2, :], axis=-1),
         )
         vs.SA_s = update(
             vs.SA_s,
             at[2:-2, 2:-2, :2, 0], 0,
         )
 
-    elif (settings.enable_chloride | settings.enable_nitrate):
+    elif (settings.enable_chloride | settings.enable_nitrate | settings.enable_virtualtracer):
         vs.msa_rz = update_multiply(
             vs.msa_rz,
             at[2:-2, 2:-2, 0, :], vs.S_rz_init[2:-2, 2:-2, npx.newaxis] / npx.sum(vs.sa_rz[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis],
         )
         vs.msa_ss = update_multiply(
             vs.msa_ss,
             at[2:-2, 2:-2, 0, :], vs.S_ss_init[2:-2, 2:-2, npx.newaxis] / npx.sum(vs.sa_ss[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis],
@@ -1287,22 +1287,8 @@
     settings = state.settings
 
     if settings.enable_offline_transport and (settings.enable_oxygen18 | settings.enable_deuterium):
         vs.update(rescale_sa_msa_iso_soil_kernel(state))
     elif settings.enable_offline_transport and (settings.enable_bromide | settings.enable_chloride | settings.enable_nitrate | settings.enable_virtualtracer):
         vs.update(rescale_sa_msa_anion_soil_kernel(state))
     elif settings.enable_offline_transport and not (settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_bromide | settings.enable_chloride | settings.enable_nitrate | settings.enable_virtualtracer):
-        vs.update(rescale_sa_soil_kernel(state))
-
-    if settings.enable_bromide:
-        vs.msa_rz = update(
-            vs.msa_rz,
-            at[2:-2, 2:-2, :2, :], 0,
-        )
-        vs.msa_ss = update(
-            vs.msa_ss,
-            at[2:-2, 2:-2, :2, :], 0,
-        )
-        vs.msa_s = update(
-            vs.msa_s,
-            at[2:-2, 2:-2, :2, :], 0,
-        )
+        vs.update(rescale_sa_soil_kernel(state))
```

### Comparing `roger-3.0/roger/core/subsoil.py` & `roger-3.0.1/roger/core/subsoil.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,29 +69,29 @@
 @roger_kernel
 def calc_S(state):
     """
     Calculates soil water content of subsoil
     """
     vs = state.variables
 
-    # horizontal redistribution
-    mask = (vs.S_fp_ss < vs.S_ufc_ss) & (vs.S_fp_ss >= 0) & (vs.S_lp_ss < vs.S_ac_ss) & (vs.S_lp_ss > 0)
-    S_fp_ss = allocate(state.dimensions, ("x", "y"))
-    S_fp_ss = update(
-        S_fp_ss,
-        at[2:-2, 2:-2], vs.S_fp_ss[2:-2, 2:-2],
-    )
-    vs.S_fp_ss = update(
-        vs.S_fp_ss,
-        at[2:-2, 2:-2], npx.where(mask[2:-2, 2:-2], npx.where((vs.S_ufc_ss[2:-2, 2:-2] - vs.S_fp_ss[2:-2, 2:-2] > vs.S_lp_ss[2:-2, 2:-2]), vs.S_fp_ss[2:-2, 2:-2] + vs.S_lp_ss[2:-2, 2:-2], vs.S_ufc_ss[2:-2, 2:-2]), vs.S_fp_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
-    )
-    vs.S_lp_ss = update(
-        vs.S_lp_ss,
-        at[2:-2, 2:-2], npx.where(mask[2:-2, 2:-2], npx.where((vs.S_ufc_ss[2:-2, 2:-2] - S_fp_ss[2:-2, 2:-2] > vs.S_lp_ss[2:-2, 2:-2]), 0, vs.S_lp_ss[2:-2, 2:-2] - (vs.S_ufc_ss[2:-2, 2:-2] - S_fp_ss[2:-2, 2:-2])), vs.S_lp_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
-    )
+    # # horizontal redistribution
+    # mask = (vs.S_fp_ss < vs.S_ufc_ss) & (vs.S_fp_ss >= 0) & (vs.S_lp_ss < vs.S_ac_ss) & (vs.S_lp_ss > 0)
+    # S_fp_ss = allocate(state.dimensions, ("x", "y"))
+    # S_fp_ss = update(
+    #     S_fp_ss,
+    #     at[2:-2, 2:-2], vs.S_fp_ss[2:-2, 2:-2],
+    # )
+    # vs.S_fp_ss = update(
+    #     vs.S_fp_ss,
+    #     at[2:-2, 2:-2], npx.where(mask[2:-2, 2:-2], npx.where((vs.S_ufc_ss[2:-2, 2:-2] - vs.S_fp_ss[2:-2, 2:-2] > vs.S_lp_ss[2:-2, 2:-2]), vs.S_fp_ss[2:-2, 2:-2] + vs.S_lp_ss[2:-2, 2:-2], vs.S_ufc_ss[2:-2, 2:-2]), vs.S_fp_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    # )
+    # vs.S_lp_ss = update(
+    #     vs.S_lp_ss,
+    #     at[2:-2, 2:-2], npx.where(mask[2:-2, 2:-2], npx.where((vs.S_ufc_ss[2:-2, 2:-2] - S_fp_ss[2:-2, 2:-2] > vs.S_lp_ss[2:-2, 2:-2]), 0, vs.S_lp_ss[2:-2, 2:-2] - (vs.S_ufc_ss[2:-2, 2:-2] - S_fp_ss[2:-2, 2:-2])), vs.S_lp_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    # )
 
     vs.S_ss = update(
         vs.S_ss,
         at[2:-2, 2:-2, vs.tau], (vs.S_pwp_ss[2:-2, 2:-2] + vs.S_fp_ss[2:-2, 2:-2] + vs.S_lp_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
     )
 
     return KernelOutput(S_ss=vs.S_ss)
```

### Comparing `roger-3.0/roger/core/subsurface_runoff.py` & `roger-3.0.1/roger/core/subsurface_runoff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1109,39 +1109,39 @@
 def calculate_percolation_rz_transport(state):
     """
     Calculates transport of percolation in root zone
     """
     vs = state.variables
     settings = state.settings
 
-    if settings.enable_offline_transport and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate):
+    if settings.enable_offline_transport and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer):
         vs.update(calc_percolation_rz_transport_kernel(state))
 
     if settings.enable_offline_transport and (settings.enable_oxygen18 | settings.enable_deuterium):
         vs.update(calc_percolation_rz_transport_iso_kernel(state))
 
-    if settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_nitrate):
+    if settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_nitrate | settings.enable_virtualtracer):
         vs.update(calc_percolation_rz_transport_anion_kernel(state))
 
 
 @roger_routine
 def calculate_percolation_ss_transport(state):
     """
     Calculates transport of percolation in subsoil
     """
     vs = state.variables
     settings = state.settings
 
-    if settings.enable_offline_transport and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate):
+    if settings.enable_offline_transport and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer):
         vs.update(calc_percolation_ss_transport_kernel(state))
 
     if settings.enable_offline_transport and (settings.enable_oxygen18 | settings.enable_deuterium):
         vs.update(calc_percolation_ss_transport_iso_kernel(state))
 
-    if settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_nitrate):
+    if settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_nitrate | settings.enable_virtualtracer):
         vs.update(calc_percolation_ss_transport_anion_kernel(state))
 
 
 @roger_kernel
 def calc_lateral_subsurface_runoff_rz_transport_kernel(state):
     """
     Calculates travel time of lateral subsurface runoff in root zone
```

### Comparing `roger-3.0/roger/core/surface.py` & `roger-3.0.1/roger/core/surface.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/core/transport.py` & `roger-3.0.1/roger/core/transport.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,31 +53,31 @@
         at[2:-2, 2:-2], npx.where(npx.max(age_dist[2:-2, 2:-2, :], axis=-1) <= 0, npx.nan, age_perc[2:-2, 2:-2]),
     )
 
     return age_perc
 
 
 @roger_kernel
-def calculate_age_statistics(state):
-    """Calculates age statistics
+def calculate_age_statistics_transp(state):
+    """Calculates age statistics of transpiration
     """
     vs = state.variables
 
     # ages in days
     ages = allocate(state.dimensions, ("x", "y", "ages"))
     ages = update(
         ages,
         at[:, :, :], npx.arange(1, ages.shape[-1]+1)[npx.newaxis, npx.newaxis, :],
     )
 
     # age statistics of transpiration
-    # vs.tt10_transp = update(
-    #     vs.tt10_transp,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_transp[:, :, 1:], 0.1)[2:-2, 2:-2],
-    # )
+    vs.tt10_transp = update(
+        vs.tt10_transp,
+        at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_transp[:, :, 1:], 0.1)[2:-2, 2:-2],
+    )
 
     vs.tt25_transp = update(
         vs.tt25_transp,
         at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_transp[:, :, 1:], 0.25)[2:-2, 2:-2],
     )
 
     vs.tt50_transp = update(
@@ -86,29 +86,45 @@
     )
 
     vs.tt75_transp = update(
         vs.tt75_transp,
         at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_transp[:, :, 1:], 0.75)[2:-2, 2:-2],
     )
 
-    # vs.tt90_transp = update(
-    #     vs.tt90_transp,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_transp[:, :, 1:], 0.9)[2:-2, 2:-2],
-    # )
+    vs.tt90_transp = update(
+        vs.tt90_transp,
+        at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_transp[:, :, 1:], 0.9)[2:-2, 2:-2],
+    )
 
     vs.ttavg_transp = update(
         vs.ttavg_transp,
         at[2:-2, 2:-2], npx.where(npx.sum(vs.tt_transp, axis=-1) > 0, npx.sum(ages * vs.tt_transp, axis=-1), npx.nan)[2:-2, 2:-2],
     )
 
+    return KernelOutput(tt10_transp=vs.tt10_transp, tt25_transp=vs.tt25_transp, tt50_transp=vs.tt50_transp, tt75_transp=vs.tt75_transp, tt90_transp=vs.tt90_transp, ttavg_transp=vs.ttavg_transp,
+                        )
+
+@roger_kernel
+def calculate_age_statistics_perc(state):
+    """Calculates age statistics of subsoil percolation
+    """
+    vs = state.variables
+
+    # ages in days
+    ages = allocate(state.dimensions, ("x", "y", "ages"))
+    ages = update(
+        ages,
+        at[:, :, :], npx.arange(1, ages.shape[-1]+1)[npx.newaxis, npx.newaxis, :],
+    )
+
     # age statistics of subsoil percolation
-    # vs.tt10_q_ss = update(
-    #     vs.tt10_q_ss,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_q_ss[:, :, 1:], 0.10)[2:-2, 2:-2],
-    # )
+    vs.tt10_q_ss = update(
+        vs.tt10_q_ss,
+        at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_q_ss[:, :, 1:], 0.10)[2:-2, 2:-2],
+    )
 
     vs.tt25_q_ss = update(
         vs.tt25_q_ss,
         at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_q_ss[:, :, 1:], 0.25)[2:-2, 2:-2],
     )
 
     vs.tt50_q_ss = update(
@@ -117,91 +133,141 @@
     )
 
     vs.tt75_q_ss = update(
         vs.tt75_q_ss,
         at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_q_ss[:, :, 1:], 0.75)[2:-2, 2:-2],
     )
 
-    # vs.tt90_q_ss = update(
-    #     vs.tt90_q_ss,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_q_ss[:, :, 1:], 0.9)[2:-2, 2:-2],
-    # )
+    vs.tt90_q_ss = update(
+        vs.tt90_q_ss,
+        at[2:-2, 2:-2], calc_age_percentile(state, vs.TT_q_ss[:, :, 1:], 0.9)[2:-2, 2:-2],
+    )
 
     vs.ttavg_q_ss = update(
         vs.ttavg_q_ss,
         at[2:-2, 2:-2], npx.where(npx.sum(vs.tt_q_ss, axis=-1) > 0, npx.sum(ages * vs.tt_q_ss, axis=-1), npx.nan)[2:-2, 2:-2],
     )
 
-    # # age statistics of root zone
-    # # cumulative residence time distribution of root zone
-    # RT_rz = allocate(state.dimensions, ("x", "y", "nages"))
-    # RT_rz = update(
-    #     RT_rz,
-    #     at[2:-2, 2:-2, :], npx.where(npx.max(vs.SA_rz[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis] > 0, vs.SA_rz[2:-2, 2:-2, vs.tau, :]/npx.max(vs.SA_rz[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis], 0),
-    # )
-    # # residence time distribution of soil
-    # rt_rz = allocate(state.dimensions, ("x", "y", "ages"))
-    # rt_rz = update(
-    #     rt_rz,
-    #     at[2:-2, 2:-2, :], npx.diff(RT_rz[2:-2, 2:-2, :], axis=-1),
-    # )
-    #
-    # vs.rt25_rz = update(
-    #     vs.rt25_rz,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, RT_rz[:, :, 1:], 0.25)[2:-2, 2:-2],
-    # )
-    #
-    # vs.rt50_rz = update(
-    #     vs.rt50_rz,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, RT_rz[:, :, 1:], 0.5)[2:-2, 2:-2],
-    # )
-    #
-    # vs.rt75_rz = update(
-    #     vs.rt75_rz,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, RT_rz[:, :, 1:], 0.75)[2:-2, 2:-2],
-    # )
-    #
-    # vs.rtavg_rz = update(
-    #     vs.rtavg_rz,
-    #     at[2:-2, 2:-2], npx.where(npx.sum(rt_rz, axis=-1) > 0, npx.sum(ages * rt_rz, axis=-1), npx.nan)[2:-2, 2:-2],
-    # )
-    #
-    # # age statistics of subsoil
-    # # cumulative residence time distribution of subsoil
-    # RT_ss = allocate(state.dimensions, ("x", "y", "nages"))
-    # RT_ss = update(
-    #     RT_ss,
-    #     at[2:-2, 2:-2, :], npx.where(npx.max(vs.SA_ss[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis] > 0, vs.SA_ss[2:-2, 2:-2, vs.tau, :]/npx.max(vs.SA_ss[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis], 0),
-    # )
-    # # residence time distribution of subsoil
-    # rt_ss = allocate(state.dimensions, ("x", "y", "ages"))
-    # rt_ss = update(
-    #     rt_ss,
-    #     at[2:-2, 2:-2, :], npx.diff(RT_ss[2:-2, 2:-2, :], axis=-1),
-    # )
-    #
-    # vs.rt25_ss = update(
-    #     vs.rt25_ss,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, RT_ss[:, :, 1:], 0.25)[2:-2, 2:-2],
-    # )
-    #
-    # vs.rt50_ss = update(
-    #     vs.rt50_ss,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, RT_ss[:, :, 1:], 0.5)[2:-2, 2:-2],
-    # )
-    #
-    # vs.rt75_ss = update(
-    #     vs.rt75_ss,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, RT_ss[:, :, 1:], 0.75)[2:-2, 2:-2],
-    # )
-    #
-    # vs.rtavg_ss = update(
-    #     vs.rtavg_ss,
-    #     at[2:-2, 2:-2], npx.where(npx.sum(rt_ss, axis=-1) > 0, npx.sum(ages * rt_ss, axis=-1), npx.nan)[2:-2, 2:-2],
-    # )
+    return KernelOutput(tt10_q_ss=vs.tt10_q_ss, tt25_q_ss=vs.tt25_q_ss, tt50_q_ss=vs.tt50_q_ss, tt75_q_ss=vs.tt75_q_ss, tt90_q_ss=vs.tt90_q_ss, ttavg_q_ss=vs.ttavg_q_ss,
+                        )
+
+
+@roger_kernel
+def calculate_age_statistics_root_zone(state):
+    """Calculates age statistics
+    """
+    vs = state.variables
+
+    # ages in days
+    ages = allocate(state.dimensions, ("x", "y", "ages"))
+    ages = update(
+        ages,
+        at[:, :, :], npx.arange(1, ages.shape[-1]+1)[npx.newaxis, npx.newaxis, :],
+    )
+
+    # age statistics of root zone
+    # cumulative residence time distribution of root zone
+    RT_rz = allocate(state.dimensions, ("x", "y", "nages"))
+    RT_rz = update(
+        RT_rz,
+        at[2:-2, 2:-2, :], npx.where(npx.max(vs.SA_rz[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis] > 0, vs.SA_rz[2:-2, 2:-2, vs.tau, :]/npx.max(vs.SA_rz[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis], 0),
+    )
+    # residence time distribution of soil
+    rt_rz = allocate(state.dimensions, ("x", "y", "ages"))
+    rt_rz = update(
+        rt_rz,
+        at[2:-2, 2:-2, :], npx.diff(RT_rz[2:-2, 2:-2, :], axis=-1),
+    )
+    
+    vs.rt25_rz = update(
+        vs.rt25_rz,
+        at[2:-2, 2:-2], calc_age_percentile(state, RT_rz[:, :, 1:], 0.25)[2:-2, 2:-2],
+    )
+    
+    vs.rt50_rz = update(
+        vs.rt50_rz,
+        at[2:-2, 2:-2], calc_age_percentile(state, RT_rz[:, :, 1:], 0.5)[2:-2, 2:-2],
+    )
+    
+    vs.rt75_rz = update(
+        vs.rt75_rz,
+        at[2:-2, 2:-2], calc_age_percentile(state, RT_rz[:, :, 1:], 0.75)[2:-2, 2:-2],
+    )
+    
+    vs.rtavg_rz = update(
+        vs.rtavg_rz,
+        at[2:-2, 2:-2], npx.where(npx.sum(rt_rz, axis=-1) > 0, npx.sum(ages * rt_rz, axis=-1), npx.nan)[2:-2, 2:-2],
+    )
+    
+
+    return KernelOutput(rt10_rz=vs.rt10_rz, rt25_rz=vs.rt25_rz, rt50_rz=vs.rt50_rz, rt75_rz=vs.rt75_rz, rt90_rz=vs.rt90_rz, rtavg_rz=vs.rtavg_rz)
+
+
+@roger_kernel
+def calculate_age_statistics_subsoil(state):
+    """Calculates age statistics
+    """
+    vs = state.variables
+
+    # ages in days
+    ages = allocate(state.dimensions, ("x", "y", "ages"))
+    ages = update(
+        ages,
+        at[:, :, :], npx.arange(1, ages.shape[-1]+1)[npx.newaxis, npx.newaxis, :],
+    )
+
+    # age statistics of subsoil
+    # cumulative residence time distribution of subsoil
+    RT_ss = allocate(state.dimensions, ("x", "y", "nages"))
+    RT_ss = update(
+        RT_ss,
+        at[2:-2, 2:-2, :], npx.where(npx.max(vs.SA_ss[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis] > 0, vs.SA_ss[2:-2, 2:-2, vs.tau, :]/npx.max(vs.SA_ss[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis], 0),
+    )
+    # residence time distribution of subsoil
+    rt_ss = allocate(state.dimensions, ("x", "y", "ages"))
+    rt_ss = update(
+        rt_ss,
+        at[2:-2, 2:-2, :], npx.diff(RT_ss[2:-2, 2:-2, :], axis=-1),
+    )
+    
+    vs.rt25_ss = update(
+        vs.rt25_ss,
+        at[2:-2, 2:-2], calc_age_percentile(state, RT_ss[:, :, 1:], 0.25)[2:-2, 2:-2],
+    )
+    
+    vs.rt50_ss = update(
+        vs.rt50_ss,
+        at[2:-2, 2:-2], calc_age_percentile(state, RT_ss[:, :, 1:], 0.5)[2:-2, 2:-2],
+    )
+    
+    vs.rt75_ss = update(
+        vs.rt75_ss,
+        at[2:-2, 2:-2], calc_age_percentile(state, RT_ss[:, :, 1:], 0.75)[2:-2, 2:-2],
+    )
+    
+    vs.rtavg_ss = update(
+        vs.rtavg_ss,
+        at[2:-2, 2:-2], npx.where(npx.sum(rt_ss, axis=-1) > 0, npx.sum(ages * rt_ss, axis=-1), npx.nan)[2:-2, 2:-2],
+    )
+
+    return KernelOutput(rt10_ss=vs.rt10_ss, rt25_ss=vs.rt25_ss, rt50_ss=vs.rt50_ss, rt75_ss=vs.rt75_ss, rt90_ss=vs.rt90_ss, rtavg_ss=vs.rtavg_ss)
+
+
+@roger_kernel
+def calculate_age_statistics_soil(state):
+    """Calculates age statistics
+    """
+    vs = state.variables
+
+    # ages in days
+    ages = allocate(state.dimensions, ("x", "y", "ages"))
+    ages = update(
+        ages,
+        at[:, :, :], npx.arange(1, ages.shape[-1]+1)[npx.newaxis, npx.newaxis, :],
+    )
 
     # age statistics of soil
     # cumulative residence time distribution of soil
     RT_s = allocate(state.dimensions, ("x", "y", "nages"))
     RT_s = update(
         RT_s,
         at[2:-2, 2:-2, :], npx.where(npx.max(vs.SA_s[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis] > 0, vs.SA_s[2:-2, 2:-2, vs.tau, :]/npx.max(vs.SA_s[2:-2, 2:-2, vs.tau, :], axis=-1)[:, :, npx.newaxis], 0),
@@ -209,18 +275,18 @@
     # residence time distribution of soil
     rt_s = allocate(state.dimensions, ("x", "y", "ages"))
     rt_s = update(
         rt_s,
         at[2:-2, 2:-2, :], npx.diff(RT_s[2:-2, 2:-2, :], axis=-1),
     )
 
-    # vs.rt10_s = update(
-    #     vs.rt10_s,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, RT_s[:, :, 1:], 0.1)[2:-2, 2:-2],
-    # )
+    vs.rt10_s = update(
+        vs.rt10_s,
+        at[2:-2, 2:-2], calc_age_percentile(state, RT_s[:, :, 1:], 0.1)[2:-2, 2:-2],
+    )
 
     vs.rt25_s = update(
         vs.rt25_s,
         at[2:-2, 2:-2], calc_age_percentile(state, RT_s[:, :, 1:], 0.25)[2:-2, 2:-2],
     )
 
     vs.rt50_s = update(
@@ -229,36 +295,25 @@
     )
 
     vs.rt75_s = update(
         vs.rt75_s,
         at[2:-2, 2:-2], calc_age_percentile(state, RT_s[:, :, 1:], 0.75)[2:-2, 2:-2],
     )
 
-    # vs.rt90_s = update(
-    #     vs.rt90_s,
-    #     at[2:-2, 2:-2], calc_age_percentile(state, RT_s[:, :, 1:], 0.9)[2:-2, 2:-2],
-    # )
+    vs.rt90_s = update(
+        vs.rt90_s,
+        at[2:-2, 2:-2], calc_age_percentile(state, RT_s[:, :, 1:], 0.9)[2:-2, 2:-2],
+    )
 
     vs.rtavg_s = update(
         vs.rtavg_s,
         at[2:-2, 2:-2], npx.where(npx.sum(rt_s, axis=-1) > 0, npx.sum(ages * rt_s, axis=-1), npx.nan)[2:-2, 2:-2],
     )
 
-    # return KernelOutput(tt25_transp=vs.tt25_transp, tt50_transp=vs.tt50_transp, tt75_transp=vs.tt75_transp, ttavg_transp=vs.ttavg_transp,
-    #                     tt25_q_ss=vs.tt25_q_ss, tt50_q_ss=vs.tt50_q_ss, tt75_q_ss=vs.tt75_q_ss, ttavg_q_ss=vs.ttavg_q_ss,
-    #                     rt25_rz=vs.rt25_rz, rt50_rz=vs.rt50_rz, rt75_rz=vs.rt75_rz, rtavg_rz=vs.rtavg_rz,
-    #                     rt25_ss=vs.rt25_ss, rt50_ss=vs.rt50_ss, rt75_ss=vs.rt75_ss, rtavg_ss=vs.rtavg_ss,
-    #                     rt25_s=vs.rt25_s, rt50_s=vs.rt50_s, rt75_s=vs.rt75_s, rtavg_s=vs.rtavg_s,
-    #                     rt10_s=vs.rt10_s, rt90_s=vs.rt90_s, tt10_transp=vs.tt10_transp,
-    #                     tt90_transp=vs.tt90_transp, tt10_q_ss=vs.tt10_q_ss, tt90_q_ss=vs.tt90_q_ss)
-    return KernelOutput(tt25_transp=vs.tt25_transp, tt50_transp=vs.tt50_transp, tt75_transp=vs.tt75_transp, ttavg_transp=vs.ttavg_transp,
-                        tt25_q_ss=vs.tt25_q_ss, tt50_q_ss=vs.tt50_q_ss, tt75_q_ss=vs.tt75_q_ss, ttavg_q_ss=vs.ttavg_q_ss,
-                        rt25_rz=vs.rt25_rz, rt50_rz=vs.rt50_rz, rt75_rz=vs.rt75_rz, rtavg_rz=vs.rtavg_rz,
-                        rt25_ss=vs.rt25_ss, rt50_ss=vs.rt50_ss, rt75_ss=vs.rt75_ss, rtavg_ss=vs.rtavg_ss,
-                        rt25_s=vs.rt25_s, rt50_s=vs.rt50_s, rt75_s=vs.rt75_s, rtavg_s=vs.rtavg_s)
+    return KernelOutput(rt10_s=vs.rt10_s, rt25_s=vs.rt25_s, rt50_s=vs.rt50_s, rt75_s=vs.rt75_s, rt90_s=vs.rt90_s, rtavg_s=vs.rtavg_s)
 
 
 @roger_kernel
 def delta_to_conc(state, delta_iso):
     """Calculate isotope concentration from isotope ratio
     """
     settings = state.settings
@@ -439,15 +494,15 @@
     tt = update(
         tt,
         at[2:-2, 2:-2, :], npx.where(flux[2:-2, 2:-2, npx.newaxis] > 0, ttq[2:-2, 2:-2, :]/flux[2:-2, 2:-2, npx.newaxis], 0),
     )
 
     if rs.backend == 'numpy':
         # sanity check of SAS function (works only for numpy backend)
-        mask = npx.isclose(npx.sum(tt, axis=-1) * flux, flux, atol=settings.atol, rtol=settings.rtol)
+        mask = npx.isclose(npx.sum(tt, axis=-1) * flux, flux, atol=0.1, rtol=0.1)
         if not npx.all(mask[2:-2, 2:-2]):
             logger.warning(f"Solution of SAS function diverged at iteration {vs.itt}.\nProbabilities of travel time distribution do not cumulate to 1.\n")
         mask2 = (tt >= 0)
         if not npx.all(mask2[2:-2, 2:-2, :]):
             logger.warning(f"Negative probabilities at iteration {vs.itt}.\n")
 
     return tt
@@ -519,15 +574,15 @@
         # solute travel time distribution at current time step
         mtt = update(
             mtt,
             at[2:-2, 2:-2, :], npx.where(tt[2:-2, 2:-2, :] > 0, msa[2:-2, 2:-2, vs.tau, :], 0),
         )
 
     # solute travel time distribution at current time step
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         mtt = update(
             mtt,
             at[2:-2, 2:-2, :], npx.where(sa[2:-2, 2:-2, vs.tau, :] > 0, (msa[2:-2, 2:-2, vs.tau, :] / sa[2:-2, 2:-2, vs.tau, :]), 0) * alpha[2:-2, 2:-2, npx.newaxis] * tt[2:-2, 2:-2, :] * flux[2:-2, 2:-2, npx.newaxis],
         )
         mtt = update(
             mtt,
             at[2:-2, 2:-2, :], npx.where(mtt[2:-2, 2:-2, :] <= 0, 0, mtt[2:-2, 2:-2, :]),
@@ -777,25 +832,25 @@
 def calculate_ageing(state):
     """
     Calculates ageing of StorAge
     """
     vs = state.variables
     settings = state.settings
 
-    if settings.enable_offline_transport and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate):
+    if settings.enable_offline_transport and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer):
         vs.update(calc_ageing_sa_kernel(state))
         if settings.enable_groundwater:
             pass
 
     elif settings.enable_offline_transport and (settings.enable_oxygen18 | settings.enable_deuterium):
         vs.update(calc_ageing_sa_msa_iso_kernel(state))
         if settings.enable_groundwater:
             pass
 
-    elif settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide):
+    elif settings.enable_offline_transport and (settings.enable_chloride | settings.enable_bromide | settings.enable_virtualtracer):
         vs.update(calc_ageing_sa_kernel(state))
         vs.update(calc_ageing_msa_kernel(state))
         if settings.enable_groundwater:
             pass
 
     elif settings.enable_offline_transport and settings.enable_nitrate:
         vs.update(calc_ageing_sa_kernel(state))
@@ -918,15 +973,19 @@
             nitrate.calculate_nitrogen_cycle(state)
     with state.timers["StorAge"]:
         root_zone.calculate_root_zone_transport(state)
         subsoil.calculate_subsoil_transport(state)
         soil.calculate_soil_transport(state)
     if settings.enable_age_statistics:
         with state.timers["age-statistics"]:
-            vs.update(calculate_age_statistics(state))
+            vs.update(calculate_age_statistics_transp(state))
+            vs.update(calculate_age_statistics_perc(state))
+            vs.update(calculate_age_statistics_root_zone(state))
+            vs.update(calculate_age_statistics_subsoil(state))
+            vs.update(calculate_age_statistics_soil(state))
     with state.timers["diagnostics"]:
         write_output(state)
     with state.timers["ageing"]:
         calculate_ageing(state)
     if settings.enable_oxygen18 or settings.enable_deuterium:
         vs.update(after_substep_iso(state))
     else:
@@ -959,15 +1018,19 @@
             nitrate.calculate_nitrogen_cycle(state)
     with state.timers["StorAge"]:
         root_zone.calculate_root_zone_transport(state)
         subsoil.calculate_subsoil_transport(state)
         soil.calculate_soil_transport(state)
     if settings.enable_age_statistics:
         with state.timers["age-statistics"]:
-            vs.update(calculate_age_statistics(state))
+            vs.update(calculate_age_statistics_transp(state))
+            vs.update(calculate_age_statistics_perc(state))
+            vs.update(calculate_age_statistics_root_zone(state))
+            vs.update(calculate_age_statistics_subsoil(state))
+            vs.update(calculate_age_statistics_soil(state))
     with state.timers["diagnostics"]:
         write_output(state)
     with state.timers["ageing"]:
         calculate_ageing(state)
     if settings.enable_oxygen18 or settings.enable_deuterium:
         vs.update(after_substep_iso(state))
     else:
@@ -992,23 +1055,27 @@
     with state.timers["infiltration into subsoil"]:
         infiltration.calculate_infiltration_ss_transport(state)
     with state.timers["percolation of subsoil"]:
         subsurface_runoff.calculate_percolation_ss_transport(state)
     with state.timers["capillary rise into root zone"]:
         capillary_rise.calculate_capillary_rise_rz_transport(state)
     if settings.enable_nitrate:
-        with state.timers["nitrogen cycle"]:
+        with state.timers["soil nitrogen cycle"]:
             nitrate.calculate_nitrogen_cycle(state)
     with state.timers["StorAge"]:
         root_zone.calculate_root_zone_transport(state)
         subsoil.calculate_subsoil_transport(state)
         soil.calculate_soil_transport(state)
     if settings.enable_age_statistics:
         with state.timers["age-statistics"]:
-            vs.update(calculate_age_statistics(state))
+            vs.update(calculate_age_statistics_transp(state))
+            vs.update(calculate_age_statistics_perc(state))
+            vs.update(calculate_age_statistics_root_zone(state))
+            vs.update(calculate_age_statistics_subsoil(state))
+            vs.update(calculate_age_statistics_soil(state))
     with state.timers["diagnostics"]:
         write_output(state)
     with state.timers["ageing"]:
         calculate_ageing(state)
     if settings.enable_oxygen18 or settings.enable_deuterium:
         vs.update(after_substep_iso(state))
     else:
@@ -1041,15 +1108,19 @@
             nitrate.calculate_nitrogen_cycle(state)
     with state.timers["StorAge"]:
         root_zone.calculate_root_zone_transport(state)
         subsoil.calculate_subsoil_transport(state)
         soil.calculate_soil_transport(state)
     if settings.enable_age_statistics:
         with state.timers["age-statistics"]:
-            vs.update(calculate_age_statistics(state))
+            vs.update(calculate_age_statistics_transp(state))
+            vs.update(calculate_age_statistics_perc(state))
+            vs.update(calculate_age_statistics_root_zone(state))
+            vs.update(calculate_age_statistics_subsoil(state))
+            vs.update(calculate_age_statistics_soil(state))
     with state.timers["diagnostics"]:
         write_output(state)
     with state.timers["ageing"]:
         calculate_ageing(state)
     if settings.enable_oxygen18 or settings.enable_deuterium:
         vs.update(after_substep_iso(state))
     else:
@@ -1139,15 +1210,15 @@
             vs.msa_rz,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, 1, :]),
         )
         vs.msa_ss = update(
             vs.msa_ss,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_ss[2:-2, 2:-2, 1, :]),
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         dsa_rz = (vs.inf_mat_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_mat_rz[2:-2, 2:-2, :] + vs.inf_pf_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_pf_rz[2:-2, 2:-2, :]) * settings.h
         dsa_ss = (vs.inf_pf_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_pf_ss[2:-2, 2:-2, :]) * settings.h
         vs.sa_rz = update_add(
             vs.sa_rz,
             at[2:-2, 2:-2, 1, :], dsa_rz,
         )
         vs.sa_ss = update_add(
@@ -1346,15 +1417,15 @@
             at[2:-2, 2:-2, 1, :], npx.where(sarkn_rz[2:-2, 2:-2, 1, :] <= 0, 0, msarkn_rz[2:-2, 2:-2, 1, :]),
         )
         msarkn_ss = update(
             msarkn_ss,
             at[2:-2, 2:-2, 1, :], npx.where(sarkn_ss[2:-2, 2:-2, 1, :] <= 0, 0, msarkn_ss[2:-2, 2:-2, 1, :]),
         )
 
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         # impose nonegative constrain to numerical solution
         dsarkn_rz = (vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * ttrkn_cpr_rz[2:-2, 2:-2, :, 0] - vs.evap_soil[2:-2, 2:-2, npx.newaxis] * ttrkn_evap_soil[2:-2, 2:-2, :, 0] - vs.transp[2:-2, 2:-2, npx.newaxis] * ttrkn_transp[2:-2, 2:-2, :, 0] - vs.q_rz[2:-2, 2:-2, npx.newaxis] * ttrkn_q_rz[2:-2, 2:-2, :, 0]) * settings.h/2
         dsarkn_rz = npx.where(sarkn_rz[2:-2, 2:-2, 1, :] + dsarkn_rz < 0, -sarkn_rz[2:-2, 2:-2, 1, :], dsarkn_rz)
         dsarkn_ss = (vs.q_rz[2:-2, 2:-2, npx.newaxis] * ttrkn_q_rz[2:-2, 2:-2, :, 0] - vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * ttrkn_cpr_rz[2:-2, 2:-2, :, 0] - vs.q_ss[2:-2, 2:-2, npx.newaxis] * ttrkn_q_ss[2:-2, 2:-2, :, 0]) * settings.h/2
         dsarkn_ss = npx.where(sarkn_ss[2:-2, 2:-2, 1, :] + dsarkn_ss < 0, -sarkn_ss[2:-2, 2:-2, 1, :], dsarkn_ss)
         sarkn_rz = update_add(
             sarkn_rz,
@@ -1495,15 +1566,15 @@
             msarkn_rz,
             at[2:-2, 2:-2, 1, :], dmsarkn_rz,
         )
         msarkn_ss = update_add(
             msarkn_ss,
             at[2:-2, 2:-2, 1, :], dmsarkn_ss,
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         # impose nonegative constrain to numerical solution
         dsarkn_rz = (vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * ttrkn_cpr_rz[2:-2, 2:-2, :, 1] - vs.evap_soil[2:-2, 2:-2, npx.newaxis] * ttrkn_evap_soil[2:-2, 2:-2, :, 1] - vs.transp[2:-2, 2:-2, npx.newaxis] * ttrkn_transp[2:-2, 2:-2, :, 1] - vs.q_rz[2:-2, 2:-2, npx.newaxis] * ttrkn_q_rz[2:-2, 2:-2, :, 1]) * settings.h/2
         dsarkn_rz = npx.where(sarkn_rz[2:-2, 2:-2, 1, :] + dsarkn_rz < 0, -sarkn_rz[2:-2, 2:-2, 1, :], dsarkn_rz)
         dsarkn_ss = (vs.q_rz[2:-2, 2:-2, npx.newaxis] * ttrkn_q_rz[2:-2, 2:-2, :, 1] - vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * ttrkn_cpr_rz[2:-2, 2:-2, :, 1] - vs.q_ss[2:-2, 2:-2, npx.newaxis] * ttrkn_q_ss[2:-2, 2:-2, :, 1]) * settings.h/2
         dsarkn_ss = npx.where(sarkn_ss[2:-2, 2:-2, 1, :] + dsarkn_ss < 0, -sarkn_ss[2:-2, 2:-2, 1, :], dsarkn_ss)
         sarkn_rz = update_add(
             sarkn_rz,
@@ -1643,15 +1714,15 @@
             msarkn_rz,
             at[2:-2, 2:-2, 1, :], dmsarkn_rz,
         )
         msarkn_ss = update_add(
             msarkn_ss,
             at[2:-2, 2:-2, 1, :], dmsarkn_ss,
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         # impose nonegative constrain to numerical solution
         dmsarkn_rz = (npx.where(npx.isnan(mttrkn_cpr_rz[2:-2, 2:-2, :, 2]), 0, mttrkn_cpr_rz[2:-2, 2:-2, :, 2]) - npx.where(npx.isnan(mttrkn_evap_soil[2:-2, 2:-2, :, 2]), 0, mttrkn_evap_soil[2:-2, 2:-2, :, 2]) - npx.where(npx.isnan(mttrkn_transp[2:-2, 2:-2, :, 2]), 0, mttrkn_transp[2:-2, 2:-2, :, 2]) - npx.where(npx.isnan(mttrkn_q_rz[2:-2, 2:-2, :, 2]), 0, mttrkn_q_rz[2:-2, 2:-2, :, 2]))
         dmsarkn_ss = (npx.where(npx.isnan(mttrkn_q_rz[2:-2, 2:-2, :, 1]), 0, mttrkn_q_rz[2:-2, 2:-2, :, 1]) - npx.where(npx.isnan(mttrkn_cpr_rz[2:-2, 2:-2, :, 1]), 0, mttrkn_cpr_rz[2:-2, 2:-2, :, 1]) - npx.where(npx.isnan(mttrkn_q_ss[2:-2, 2:-2, :, 1]), 0, mttrkn_q_ss[2:-2, 2:-2, :, 1]))
         dmsarkn_rz = npx.where(msarkn_rz[2:-2, 2:-2, 1, :] - dmsarkn_rz < 0, -msarkn_rz[2:-2, 2:-2, 1, :], dmsarkn_rz)
         dmsarkn_ss = npx.where(msarkn_ss[2:-2, 2:-2, 1, :] - dmsarkn_ss < 0, -msarkn_ss[2:-2, 2:-2, 1, :], dmsarkn_ss)
         msarkn_rz = update_add(
             msarkn_rz,
@@ -1855,15 +1926,15 @@
             vs.msa_rz,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, 1, :]),
         )
         vs.msa_ss = update(
             vs.msa_ss,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_ss[2:-2, 2:-2, 1, :]),
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         # impose nonegative constrain of numerical solution
         dsa_rz = (vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :] - vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :] - vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :]) * settings.h
         dsa_rz = npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] + dsa_rz < 0, -vs.sa_rz[2:-2, 2:-2, 1, :], dsa_rz)
         dsa_ss = (vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :] - vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :] - vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :]) * settings.h
         dsa_ss = npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] + dsa_ss < 0, -vs.sa_ss[2:-2, 2:-2, 1, :], dsa_ss)
         vs.sa_rz = update_add(
             vs.sa_rz,
@@ -1926,15 +1997,15 @@
             at[2:-2, 2:-2], calc_conc_iso_flux(state, vs.mtt_cpr_rz, vs.tt_cpr_rz, vs.cpr_rz)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
         )
         vs.C_q_ss = update(
             vs.C_q_ss,
             at[2:-2, 2:-2], calc_conc_iso_flux(state, vs.mtt_q_ss, vs.tt_q_ss, vs.q_ss)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
         )
 
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         vs.C_inf_mat_rz = update(
             vs.C_inf_mat_rz,
             at[2:-2, 2:-2], npx.where(vs.inf_mat_rz[2:-2, 2:-2] > 0, vs.C_in[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
         )
         vs.C_inf_pf_rz = update(
             vs.C_inf_pf_rz,
             at[2:-2, 2:-2], npx.where(vs.inf_pf_rz[2:-2, 2:-2] > 0, vs.C_in[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
@@ -2064,15 +2135,15 @@
             vs.msa_rz,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, 1, :]),
         )
         vs.msa_ss = update(
             vs.msa_ss,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_ss[2:-2, 2:-2, 1, :]),
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         dsa_rz = (vs.inf_mat_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_mat_rz[2:-2, 2:-2, :] + vs.inf_pf_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_pf_rz[2:-2, 2:-2, :]) * settings.h
         dsa_ss = (vs.inf_pf_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_pf_ss[2:-2, 2:-2, :]) * settings.h
         vs.sa_rz = update_add(
             vs.sa_rz,
             at[2:-2, 2:-2, 1, :], dsa_rz,
         )
         vs.sa_ss = update_add(
@@ -2222,15 +2293,15 @@
             vs.msa_rz,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, 1, :]),
         )
         vs.msa_ss = update(
             vs.msa_ss,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_ss[2:-2, 2:-2, 1, :]),
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         # impose nonegative constrain of numerical solution
         dsa_rz = (vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :] - vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :] - vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :] - vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :]) * settings.h
         dsa_rz = npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] + dsa_rz < 0, -vs.sa_rz[2:-2, 2:-2, 1, :], dsa_rz)
         dsa_ss = (vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :] - vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :] - vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :]) * settings.h
         dsa_ss = npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] + dsa_ss < 0, -vs.sa_ss[2:-2, 2:-2, 1, :], dsa_ss)
         vs.sa_rz = update_add(
             vs.sa_rz,
@@ -2293,15 +2364,15 @@
             at[2:-2, 2:-2], calc_conc_iso_flux(state, vs.mtt_cpr_rz, vs.tt_cpr_rz, vs.cpr_rz)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
         )
         vs.C_q_ss = update(
             vs.C_q_ss,
             at[2:-2, 2:-2], calc_conc_iso_flux(state, vs.mtt_q_ss, vs.tt_q_ss, vs.q_ss)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
         )
 
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         vs.C_inf_mat_rz = update(
             vs.C_inf_mat_rz,
             at[2:-2, 2:-2], npx.where(vs.inf_mat_rz[2:-2, 2:-2] > 0, vs.C_in[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
         )
         vs.C_inf_pf_rz = update(
             vs.C_inf_pf_rz,
             at[2:-2, 2:-2], npx.where(vs.inf_pf_rz[2:-2, 2:-2] > 0, vs.C_in[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
@@ -2430,15 +2501,15 @@
             vs.msa_rz,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, 1, :]),
         )
         vs.msa_ss = update(
             vs.msa_ss,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_ss[2:-2, 2:-2, 1, :]),
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         dsa_rz = (vs.inf_mat_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_mat_rz[2:-2, 2:-2, :] + vs.inf_pf_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_pf_rz[2:-2, 2:-2, :]) * settings.h
         dsa_ss = (vs.inf_pf_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_pf_ss[2:-2, 2:-2, :]) * settings.h
         vs.sa_rz = update_add(
             vs.sa_rz,
             at[2:-2, 2:-2, 1, :], dsa_rz,
         )
         vs.sa_ss = update_add(
@@ -2568,15 +2639,15 @@
             vs.msa_rz,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, 1, :]),
         )
         vs.msa_ss = update(
             vs.msa_ss,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_ss[2:-2, 2:-2, 1, :]),
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         # impose nonegative constrain of numerical solution
         dsa_rz = (vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :] - vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :] - vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :] - vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :]) * settings.h
         dsa_rz = npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] + dsa_rz < 0, -vs.sa_rz[2:-2, 2:-2, 1, :], dsa_rz)
         dsa_ss = (vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :] + vs.cpr_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_ss[2:-2, 2:-2, :] - vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :] - vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :]) * settings.h
         dsa_ss = npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] + dsa_ss < 0, -vs.sa_ss[2:-2, 2:-2, 1, :], dsa_ss)
         vs.sa_rz = update_add(
             vs.sa_rz,
@@ -2638,15 +2709,15 @@
             at[2:-2, 2:-2], calc_conc_iso_flux(state, vs.mtt_cpr_rz, vs.tt_cpr_rz, vs.cpr_rz)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
         )
         vs.C_q_ss = update(
             vs.C_q_ss,
             at[2:-2, 2:-2], calc_conc_iso_flux(state, vs.mtt_q_ss, vs.tt_q_ss, vs.q_ss)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
         )
 
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         vs.C_inf_mat_rz = update(
             vs.C_inf_mat_rz,
             at[2:-2, 2:-2], npx.where(vs.inf_mat_rz[2:-2, 2:-2] > 0, vs.C_in[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
         )
         vs.C_inf_pf_rz = update(
             vs.C_inf_pf_rz,
             at[2:-2, 2:-2], npx.where(vs.inf_pf_rz[2:-2, 2:-2] > 0, vs.C_in[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
@@ -2762,15 +2833,15 @@
             vs.msa_rz,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, 1, :]),
         )
         vs.msa_ss = update(
             vs.msa_ss,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_ss[2:-2, 2:-2, 1, :]),
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         dsa_rz = (vs.inf_mat_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_mat_rz[2:-2, 2:-2, :] + vs.inf_pf_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_pf_rz[2:-2, 2:-2, :]) * settings.h
         dsa_ss = (vs.inf_pf_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_inf_pf_ss[2:-2, 2:-2, :]) * settings.h
         vs.sa_rz = update_add(
             vs.sa_rz,
             at[2:-2, 2:-2, 1, :], dsa_rz,
         )
         vs.sa_ss = update_add(
@@ -2924,15 +2995,15 @@
             vs.msa_rz,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_rz[2:-2, 2:-2, 1, :]),
         )
         vs.msa_ss = update(
             vs.msa_ss,
             at[2:-2, 2:-2, 1, :], npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] <= 0, 0, vs.msa_ss[2:-2, 2:-2, 1, :]),
         )
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         # impose nonegative constrain of numerical solution
         dsa_rz = (vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :] + vs.q_re_rg[2:-2, 2:-2, npx.newaxis] * vs.tt_re_rg[2:-2, 2:-2, :] - vs.evap_soil[2:-2, 2:-2, npx.newaxis] * vs.tt_evap_soil[2:-2, 2:-2, :] - vs.transp[2:-2, 2:-2, npx.newaxis] * vs.tt_transp[2:-2, 2:-2, :] - vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :] - vs.q_re_rl[2:-2, 2:-2, npx.newaxis] * vs.tt_re_rl[2:-2, 2:-2, :]) * settings.h
         dsa_rz = npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] + dsa_rz < 0, -vs.sa_rz[2:-2, 2:-2, 1, :], dsa_rz)
         dsa_rz = npx.where(vs.sa_rz[2:-2, 2:-2, 1, :] + dsa_rz < 0, -vs.sa_rz[2:-2, 2:-2, 1, :], dsa_rz)
         dsa_ss = (vs.q_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_q_rz[2:-2, 2:-2, :] + vs.q_re_rl[2:-2, 2:-2, npx.newaxis] * vs.tt_re_rl[2:-2, 2:-2, :] - vs.cpr_rz[2:-2, 2:-2, npx.newaxis] * vs.tt_cpr_rz[2:-2, 2:-2, :] - vs.q_ss[2:-2, 2:-2, npx.newaxis] * vs.tt_q_ss[2:-2, 2:-2, :] - vs.q_re_rg[2:-2, 2:-2, npx.newaxis] * vs.tt_re_rg[2:-2, 2:-2, :]) * settings.h
         dsa_ss = npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] + dsa_ss < 0, -vs.sa_ss[2:-2, 2:-2, 1, :], dsa_ss)
         dsa_ss = npx.where(vs.sa_ss[2:-2, 2:-2, 1, :] + dsa_ss < 0, -vs.sa_ss[2:-2, 2:-2, 1, :], dsa_ss)
@@ -3004,15 +3075,15 @@
             at[2:-2, 2:-2], calc_conc_iso_flux(state, vs.mtt_re_rg, vs.tt_re_rg, vs.re_rg)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
         )
         vs.C_re_rl = update(
             vs.C_re_rl,
             at[2:-2, 2:-2], calc_conc_iso_flux(state, vs.mtt_re_rl, vs.tt_re_rl, vs.re_rl)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
         )
 
-    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate:
+    elif settings.enable_bromide or settings.enable_chloride or settings.enable_nitrate or settings.enable_virtualtracer:
         vs.C_inf_mat_rz = update(
             vs.C_inf_mat_rz,
             at[2:-2, 2:-2], npx.where(vs.inf_mat_rz[2:-2, 2:-2] > 0, vs.C_in[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
         )
         vs.C_inf_pf_rz = update(
             vs.C_inf_pf_rz,
             at[2:-2, 2:-2], npx.where(vs.inf_pf_rz[2:-2, 2:-2] > 0, vs.C_in[2:-2, 2:-2], 0) * vs.maskCatch[2:-2, 2:-2],
@@ -3056,26 +3127,30 @@
 @roger_routine
 def calculate_storage_selection(state):
     """Calculates transport model
     """
     vs = state.variables
     settings = state.settings
 
-    if settings.enable_offline_transport and not (settings.enable_groundwater_boundary & settings.enable_crop_phenology) and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate):
+    if settings.enable_offline_transport and not settings.enable_groundwater_boundary and not settings.enable_crop_phenology and not (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer):
         if settings.sas_solver == "Euler":
             # loop over substeps
             for i in range(settings.sas_solver_substeps):
                 vs.update(svat_transport_model_euler(state))
                 root_zone.calculate_root_zone_transport(state)
                 subsoil.calculate_subsoil_transport(state)
                 soil.calculate_soil_transport(state)
                 vs.time = vs.time + int(vs.dt_secs / settings.sas_solver_substeps)
                 if settings.enable_age_statistics:
                     with state.timers["age-statistics"]:
-                        vs.update(calculate_age_statistics(state))
+                        vs.update(calculate_age_statistics_transp(state))
+                        vs.update(calculate_age_statistics_perc(state))
+                        vs.update(calculate_age_statistics_root_zone(state))
+                        vs.update(calculate_age_statistics_subsoil(state))
+                        vs.update(calculate_age_statistics_soil(state))
                 # collect data for output at end of substep
                 with state.timers["diagnostics"]:
                     write_output(state)
                 if (vs.time % (24 * 60 * 60) == 0):
                     calculate_ageing(state)
                     vs.update(after_substep_anion(state))
                 else:
@@ -3088,43 +3163,51 @@
                 vs.update(svat_transport_model_rk4(state))
                 root_zone.calculate_root_zone_transport(state)
                 subsoil.calculate_subsoil_transport(state)
                 soil.calculate_soil_transport(state)
                 vs.time = vs.time + int(vs.dt_secs / settings.sas_solver_substeps)
                 if settings.enable_age_statistics:
                     with state.timers["age-statistics"]:
-                        vs.update(calculate_age_statistics(state))
+                        vs.update(calculate_age_statistics_transp(state))
+                        vs.update(calculate_age_statistics_perc(state))
+                        vs.update(calculate_age_statistics_root_zone(state))
+                        vs.update(calculate_age_statistics_subsoil(state))
+                        vs.update(calculate_age_statistics_soil(state))
                 # collect data for output at end of substep
                 with state.timers["diagnostics"]:
                     write_output(state)
                 if (vs.time % (24 * 60 * 60) == 0):
                     calculate_ageing(state)
                     vs.update(after_substep_anion(state))
                 else:
                     vs.update(after_substep_anion(state))
                 vs.itt_substep = i
 
         else:
             vs.update(svat_transport_model_deterministic(state))
 
-    elif settings.enable_offline_transport and not (settings.enable_groundwater_boundary & settings.enable_crop_phenology) and (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate):
+    elif settings.enable_offline_transport and not settings.enable_groundwater_boundary and not settings.enable_crop_phenology and (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer):
         if settings.sas_solver == "Euler":
             # loop over substeps
             for i in range(settings.sas_solver_substeps):
                 vs.update(svat_transport_model_euler(state))
                 if (settings.enable_oxygen18 | settings.enable_deuterium):
                     # convert isotope concentrations to delta valus
                     vs.update(delta_fluxes_svat(state))
                 root_zone.calculate_root_zone_transport(state)
                 subsoil.calculate_subsoil_transport(state)
                 soil.calculate_soil_transport(state)
                 vs.time = vs.time + int(vs.dt_secs / settings.sas_solver_substeps)
                 if settings.enable_age_statistics:
                     with state.timers["age-statistics"]:
-                        vs.update(calculate_age_statistics(state))
+                        vs.update(calculate_age_statistics_transp(state))
+                        vs.update(calculate_age_statistics_perc(state))
+                        vs.update(calculate_age_statistics_root_zone(state))
+                        vs.update(calculate_age_statistics_subsoil(state))
+                        vs.update(calculate_age_statistics_soil(state))
                 # collect data for output at end of substep
                 with state.timers["diagnostics"]:
                     write_output(state)
                 if (vs.time % (24 * 60 * 60) == 0):
                     calculate_ageing(state)
                     if (settings.enable_oxygen18 | settings.enable_deuterium):
                         vs.update(after_substep_iso(state))
@@ -3146,15 +3229,19 @@
                     vs.update(delta_fluxes_svat(state))
                 root_zone.calculate_root_zone_transport(state)
                 subsoil.calculate_subsoil_transport(state)
                 soil.calculate_soil_transport(state)
                 vs.time = vs.time + int(vs.dt_secs / settings.sas_solver_substeps)
                 if settings.enable_age_statistics:
                     with state.timers["age-statistics"]:
-                        vs.update(calculate_age_statistics(state))
+                        vs.update(calculate_age_statistics_transp(state))
+                        vs.update(calculate_age_statistics_perc(state))
+                        vs.update(calculate_age_statistics_root_zone(state))
+                        vs.update(calculate_age_statistics_subsoil(state))
+                        vs.update(calculate_age_statistics_soil(state))
                 # collect data for output at end of substep
                 with state.timers["diagnostics"]:
                     write_output(state)
                 if (vs.time % (24 * 60 * 60) == 0):
                     calculate_ageing(state)
                     if (settings.enable_oxygen18 | settings.enable_deuterium):
                         vs.update(after_substep_iso(state))
@@ -3166,29 +3253,33 @@
                     else:
                         vs.update(after_substep_anion(state))
                 vs.itt_substep = i
 
         else:
             vs.update(svat_transport_model_deterministic(state))
 
-    elif settings.enable_offline_transport and settings.enable_groundwater_boundary and not settings.enable_crop_phenology and (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate):
+    elif settings.enable_offline_transport and settings.enable_groundwater_boundary and not settings.enable_crop_phenology and (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer):
         if settings.sas_solver == "Euler":
             # loop over substeps
             for i in range(settings.sas_solver_substeps):
                 vs.update(svat_lbc_transport_model_euler(state))
                 if (settings.enable_oxygen18 | settings.enable_deuterium):
                     # convert isotope concentrations to delta valus
                     vs.update(delta_fluxes_svat(state))
                 root_zone.calculate_root_zone_transport(state)
                 subsoil.calculate_subsoil_transport(state)
                 soil.calculate_soil_transport(state)
                 vs.time = vs.time + int(vs.dt_secs / settings.sas_solver_substeps)
                 if settings.enable_age_statistics:
                     with state.timers["age-statistics"]:
-                        vs.update(calculate_age_statistics(state))
+                        vs.update(calculate_age_statistics_transp(state))
+                        vs.update(calculate_age_statistics_perc(state))
+                        vs.update(calculate_age_statistics_root_zone(state))
+                        vs.update(calculate_age_statistics_subsoil(state))
+                        vs.update(calculate_age_statistics_soil(state))
                 # collect data for output at end of substep
                 with state.timers["diagnostics"]:
                     write_output(state)
                 if (vs.time % (24 * 60 * 60) == 0):
                     calculate_ageing(state)
                     if (settings.enable_oxygen18 | settings.enable_deuterium):
                         vs.update(after_substep_iso(state))
@@ -3203,29 +3294,33 @@
 
         elif settings.sas_solver == "RK4":
             pass
 
         else:
             vs.update(svat_lbc_transport_model_deterministic(state))
 
-    elif settings.enable_offline_transport and not settings.enable_groundwater_boundary and settings.enable_crop_phenology and (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate):
+    elif settings.enable_offline_transport and not settings.enable_groundwater_boundary and settings.enable_crop_phenology and (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer):
         if settings.sas_solver == "Euler":
             # loop over substeps
             for i in range(settings.sas_solver_substeps):
                 vs.update(svat_crop_transport_model_euler(state))
                 if (settings.enable_oxygen18 | settings.enable_deuterium):
                     # convert isotope concentrations to delta valus
                     vs.update(delta_fluxes_svat_crop(state))
                 root_zone.calculate_root_zone_transport(state)
                 subsoil.calculate_subsoil_transport(state)
                 soil.calculate_soil_transport(state)
                 vs.time = vs.time + int(vs.dt_secs / settings.sas_solver_substeps)
                 if settings.enable_age_statistics:
                     with state.timers["age-statistics"]:
-                        vs.update(calculate_age_statistics(state))
+                        vs.update(calculate_age_statistics_transp(state))
+                        vs.update(calculate_age_statistics_perc(state))
+                        vs.update(calculate_age_statistics_root_zone(state))
+                        vs.update(calculate_age_statistics_subsoil(state))
+                        vs.update(calculate_age_statistics_soil(state))
                 # collect data for output at end of substep
                 with state.timers["diagnostics"]:
                     write_output(state)
                 if (vs.time % (24 * 60 * 60) == 0):
                     calculate_ageing(state)
                     if (settings.enable_oxygen18 | settings.enable_deuterium):
                         vs.update(after_substep_iso(state))
@@ -3248,19 +3343,21 @@
 @roger_routine
 def write_output(state):
     """Collect and write output
     """
     vs = state.variables
     settings = state.settings
 
-    if not numerics.sanity_check(state):
+    if not numerics.sanity_check(state) and not settings.warmup_done:
+        logger.warning(f"Solution diverged at iteration {vs.itt} at substep {vs.itt_substep}.")
+    elif not numerics.sanity_check(state) and settings.warmup_done:
         logger.warning(f"Solution diverged at iteration {vs.itt} at substep {vs.itt_substep}.\n An evaluation of the bias of the deterministic/numerical\n solution is highly recommended. The bias is written to\n the model output.")
-    numerics.calculate_num_error(state)
 
     if settings.warmup_done:
+        numerics.calculate_num_error(state)
         diagnostics.diagnose(state)
         diagnostics.output(state)
 
 
 @roger_kernel
 def after_substep_iso(state):
     vs = state.variables
```

### Comparing `roger-3.0/roger/core/utilities.py` & `roger-3.0.1/roger/core/utilities.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/api.py` & `roger-3.0.1/roger/diagnostics/api.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/average.py` & `roger-3.0.1/roger/diagnostics/average.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/base.py` & `roger-3.0.1/roger/diagnostics/base.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/collect.py` & `roger-3.0.1/roger/diagnostics/collect.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/constant.py` & `roger-3.0.1/roger/diagnostics/constant.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/maximum.py` & `roger-3.0.1/roger/diagnostics/maximum.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/minimum.py` & `roger-3.0.1/roger/diagnostics/minimum.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/rate.py` & `roger-3.0.1/roger/diagnostics/rate.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/snapshot.py` & `roger-3.0.1/roger/diagnostics/snapshot.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/tracer_monitor.py` & `roger-3.0.1/roger/diagnostics/tracer_monitor.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/diagnostics/water_monitor.py` & `roger-3.0.1/roger/diagnostics/water_monitor.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/distributed.py` & `roger-3.0.1/roger/distributed.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/io_tools/csv.py` & `roger-3.0.1/roger/io_tools/csv.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/io_tools/hdf5.py` & `roger-3.0.1/roger/io_tools/hdf5.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/io_tools/netcdf.py` & `roger-3.0.1/roger/io_tools/netcdf.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/io_tools/yml.py` & `roger-3.0.1/roger/io_tools/yml.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/logs.py` & `roger-3.0.1/roger/logs.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/lookuptables.py` & `roger-3.0.1/roger/lookuptables.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/models/dummy/dummy.py` & `roger-3.0.1/roger/models/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/models/oneD/oneD.py` & `roger-3.0.1/roger/models/oneD/oneD.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/models/oneD_event/oneD_event.py` & `roger-3.0.1/roger/models/oneD_event/oneD_event.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/models/svat/svat.py` & `roger-3.0.1/roger/models/svat/svat.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/models/svat_bromide/svat_bromide.py` & `roger-3.0.1/roger/models/svat_bromide/svat_bromide.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/models/svat_crop/svat_crop.py` & `roger-3.0.1/roger/models/svat_crop/svat_crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,18 +157,18 @@
         vs.ks = update(vs.ks, at[2:-2, 2:-2], 5)
         vs.kf = update(vs.kf, at[2:-2, 2:-2], 2500)
 
         vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 0], 564)
         vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 1], 539)
         vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 2], 564)
 
-        vs.z_root = update(vs.z_root, at[2:-2, 2:-2, :2], 400)
+        vs.z_root = update(vs.z_root, at[2:-2, 2:-2, :2], 200)
         vs.z_root_crop = update(
             vs.z_root_crop,
-            at[2:-2, 2:-2, :2, 0], 400
+            at[2:-2, 2:-2, :2, 0], 200
         )
 
     @roger_routine
     def set_parameters(self, state):
         vs = state.variables
 
         if (vs.month[vs.tau] != vs.month[vs.taum1]) & (vs.itt > 1):
@@ -470,29 +470,36 @@
         doy=vs.doy,
         S_fp_rz=vs.S_fp_rz,
         S_lp_rz=vs.S_lp_rz,
         S_fp_ss=vs.S_fp_ss,
         S_lp_ss=vs.S_lp_ss,
     )
 
-
 @roger_kernel
 def after_timestep_crops_kernel(state):
     vs = state.variables
 
     vs.ta_min = update(vs.ta_min, at[2:-2, 2:-2, vs.taum1], vs.ta_min[2:-2, 2:-2, vs.tau])
     vs.ta_max = update(vs.ta_max, at[2:-2, 2:-2, vs.taum1], vs.ta_max[2:-2, 2:-2, vs.tau])
     vs.gdd_sum = update(vs.gdd_sum, at[2:-2, 2:-2, vs.taum1, :], vs.gdd_sum[2:-2, 2:-2, vs.tau, :])
     vs.t_grow_cc = update(vs.t_grow_cc, at[2:-2, 2:-2, vs.taum1, :], vs.t_grow_cc[2:-2, 2:-2, vs.tau, :])
     vs.t_grow_root = update(vs.t_grow_root, at[2:-2, 2:-2, vs.taum1, :], vs.t_grow_root[2:-2, 2:-2, vs.tau, :])
     vs.ccc = update(vs.ccc, at[2:-2, 2:-2, vs.taum1, :], vs.ccc[2:-2, 2:-2, vs.tau, :])
     vs.z_root_crop = update(vs.z_root_crop, at[2:-2, 2:-2, vs.taum1, :], vs.z_root_crop[2:-2, 2:-2, vs.tau, :])
+    vs.re_rg_pwp = update(vs.re_rg_pwp, at[2:-2, 2:-2], 0)
+    vs.re_rg = update(vs.re_rg, at[2:-2, 2:-2], 0)
+    vs.re_rl_pwp = update(vs.re_rl_pwp, at[2:-2, 2:-2], 0)
+    vs.re_rl = update(vs.re_rl, at[2:-2, 2:-2], 0)
 
     return KernelOutput(
         ta_min=vs.ta_min,
         ta_max=vs.ta_max,
         gdd_sum=vs.gdd_sum,
         t_grow_cc=vs.t_grow_cc,
         t_grow_root=vs.t_grow_root,
         ccc=vs.ccc,
         z_root_crop=vs.z_root_crop,
+        re_rg_pwp=vs.re_rg_pwp,
+        re_rg=vs.re_rg,
+        re_rl_pwp=vs.re_rl_pwp,
+        re_rl=vs.re_rl,
     )
```

### Comparing `roger-3.0/roger/models/svat_oxygen18/svat_oxygen18.py` & `roger-3.0.1/roger/models/svat_oxygen18/svat_oxygen18.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/plugins.py` & `roger-3.0.1/roger/plugins.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/progress.py` & `roger-3.0.1/roger/progress.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/restart.py` & `roger-3.0.1/roger/restart.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/roger.py` & `roger-3.0.1/roger/roger.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 
         if self.state.settings.warmup_done:
             # write initial values to output
             diagnostics.diagnose(self.state)
             diagnostics.output(self.state)
 
         logger.success("Setup done\n")
-        if (self.state.settings.enable_chloride | self.state.settings.enable_bromide | self.state.settings.enable_oxygen18 | self.state.settings.enable_deuterium | self.state.settings.enable_nitrate):
+        if (self.state.settings.enable_chloride | self.state.settings.enable_bromide | self.state.settings.enable_oxygen18 | self.state.settings.enable_deuterium | self.state.settings.enable_nitrate | self.state.settings.enable_virtualtracer):
             logger.warning("IMPORTANT: Always check your logger output for warnings\n on diverging solutions. The occurence of warnings may\n require an post-evaluation of the accuracy of\n the numerical solution (e.g. calculate\n standard deviation of dS_num_error or dC_num_error).\n")
         else:
             logger.warning("IMPORTANT: Always check your logger output for warnings\n on diverging solutions. The occurence of warnings may\n require an post-evaluation of the accuracy of\n the numerical solution (e.g. calculate\n standard deviation of dS_num_error).\n")
 
     @roger_routine
     def step(self, state):
         from roger import diagnostics, restart
@@ -355,14 +355,17 @@
                     with state.timers["adaptive time-stepping"]:
                         adaptive_time_stepping.adaptive_time_stepping(state)
                 with state.timers["time-variant parameters"]:
                     self.set_parameters(state)
                 if settings.enable_crop_phenology:
                     with state.timers["crops"]:
                         crop.calculate_crop_phenology(state)
+                        root_zone.calculate_root_zone(state)
+                        subsoil.calculate_subsoil(state)
+                        soil.calculate_soil(state)
                 with state.timers["interception"]:
                     interception.calculate_interception(state)
                 with state.timers["evapotranspiration"]:
                     evapotranspiration.calculate_evapotranspiration(state)
                 with state.timers["snow"]:
                     snow.calculate_snow(state)
                 with state.timers["infiltration"]:
```

### Comparing `roger-3.0/roger/routines.py` & `roger-3.0.1/roger/routines.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/runtime.py` & `roger-3.0.1/roger/runtime.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/settings.py` & `roger-3.0.1/roger/settings.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/signals.py` & `roger-3.0.1/roger/signals.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/state.py` & `roger-3.0.1/roger/state.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/time.py` & `roger-3.0.1/roger/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     all_units = X_TO_SECONDS.keys()
     val_in_all_units = {u: convert_time(time_value, in_unit, u) for u in all_units}
     valid_units = {u: v for u, v in val_in_all_units.items() if v >= 1.0}
     if valid_units:
         best_unit = min(valid_units, key=valid_units.get)
     else:
         best_unit = "seconds"
-    return val_in_all_units[best_unit], best_unit
+    return round(val_in_all_units[best_unit], 2), best_unit
```

### Comparing `roger-3.0/roger/tools/evaluation.py` & `roger-3.0.1/roger/tools/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
     # Plot the lines on facets
     g = sns.relplot(
         data=df_sim_obs_long,
         x="time", y="value",
         hue="type", col="hyd_year",
         kind="line", palette=palette,
         facet_kws=dict(sharex=False),
-        height=4, aspect=.7, col_wrap=4
+        height=1.5, aspect=1, col_wrap=4
     )
     g.set_ylabels(y_lab)
     g.set_xlabels(x_lab)
     g.set_xticklabels(rotation=90)
     for axs in g.axes.flatten():
         axs.xaxis.set_major_formatter(mdates.DateFormatter('%d-%m'))
     g.set_titles(template='{col_name}')
@@ -480,15 +480,15 @@
     # Plot the lines on facets
     g = sns.relplot(
         data=df_sim_long,
         x="time", y="value",
         hue="type", col="hyd_year",
         kind="line", palette=palette,
         facet_kws=dict(sharex=False),
-        height=4, aspect=.7, col_wrap=4
+        height=1.5, aspect=1, col_wrap=4
     )
     g.set_ylabels(y_lab)
     g.set_xlabels(x_lab)
     g.set_xticklabels(rotation=90)
     for axs in g.axes.flatten():
         axs.xaxis.set_major_formatter(mdates.DateFormatter('%d-%m'))
     g.set_titles(template='{col_name}')
```

### Comparing `roger-3.0/roger/tools/event_classification.py` & `roger-3.0.1/roger/tools/event_classification.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/tools/filelock.py` & `roger-3.0.1/roger/tools/filelock.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/tools/labels.py` & `roger-3.0.1/roger/tools/labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,15 @@
          'dz_sat_ss': r'$\Delta z_{ss-sat}$ [mm]',
          'z0': r'$z_{0}$ [mm]',
          'z_sat': r'$z_{sat}$ [mm]',
          'y_mp': r'$y_{mp}$ [mm]',
          'z_sc': r'$z_{sc}$ [mm]',
          'y_sc': r'$y_{sc}$ [mm]',
          'z_wf': r'$z_{wf}$ [mm]',
+         'z_soil': r'$z_{soil}$ [mm]',
          'z_wf_t0': r'$z_{wf}(t_0)$ [mm]',
          'z_wf_t1': r'$z_{wf}(t_1)$ [mm]',
          'z_sat_rz': r'$z_{sat-rz}$ [mm]',
          'z_sat_ss': r'$z_{sat-ss}$ [mm]',
          'z_sat': r'$z_{sat}$ [mm]',
          'z_gw': r'$z_{gw}$ [m]',
          'z_root': r'$z_{root}$ [mm]',
```

### Comparing `roger-3.0/roger/tools/make_toy_data.py` & `roger-3.0.1/roger/tools/make_toy_data.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/roger/tools/setup.py` & `roger-3.0.1/roger/tools/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
         v = f.create_variable('crop', ('x', 'y', 'year_season'), int)
         v[:, :,  :] = arr
         v.attrs['long_name'] = 'crop'
         v.attrs['units'] = ''
         v = f.create_variable('year_season', ('year_season',), 'S11')
         v.attrs['units'] = 'year_season'
-        v[:] = onp.array(crops.columns[1:].astype('S11').values, dtype='S11')
+        v[:] = onp.array(crops.columns[1:].astype('U11').values, dtype='S11')
         v = f.create_variable('x', ('x',), float_type)
         v.attrs['long_name'] = 'Zonal coordinate'
         v.attrs['units'] = 'meters'
         v[:] = onp.arange(nrows)
         v = f.create_variable('y', ('y',), float_type)
         v.attrs['long_name'] = 'Meridonial coordinate'
         v.attrs['units'] = 'meters'
```

### Comparing `roger-3.0/roger/variables.py` & `roger-3.0.1/roger/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,14 +679,28 @@
     "TA": Variable(
         "air temperature",
         TIME_FORCING,
         "degC",
         "air temperature",
         active=lambda settings: not settings.enable_offline_transport,
     ),
+    "TA_MIN": Variable(
+        "daily minimum air temperature",
+        TIME_FORCING,
+        "degC",
+        "daily minimum air temperature",
+        active=lambda settings: not settings.enable_offline_transport and settings.enable_crop_phenology,
+    ),
+    "TA_MAX": Variable(
+        "daily maximum air temperature",
+        TIME_FORCING,
+        "degC",
+        "daily maximum air temperature",
+        active=lambda settings: not settings.enable_offline_transport and settings.enable_crop_phenology,
+    ),
     "ta": Variable(
         "air temperature",
         CATCH_GRID + TIMESTEPS,
         "degC",
         "air temperature",
         time_dependent=True,
     ),
@@ -2200,14 +2214,22 @@
         CATCH_GRID + TIMESTEPS,
         "per mil",
         "isotope ratio of root zone",
         time_dependent=True,
         write_to_restart=True,
         active=lambda settings: settings.enable_offline_transport & (settings.enable_oxygen18 | settings.enable_deuterium),
     ),
+    "rt10_rz": Variable(
+        "10th percentile of root zone residence time",
+        CATCH_GRID,
+        "days",
+        "10th percentile of root zone residence time",
+        time_dependent=True,
+        active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
+    ),
     "rt25_rz": Variable(
         "25th percentile of root zone residence time",
         CATCH_GRID,
         "days",
         "25th percentile of root zone residence time",
         time_dependent=True,
         active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
@@ -2224,14 +2246,22 @@
         "75th percentile of root zone residence time",
         CATCH_GRID,
         "days",
         "75th percentile of root zone residence time",
         time_dependent=True,
         active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
     ),
+    "rt90_rz": Variable(
+        "90th percentile of root zone residence time",
+        CATCH_GRID,
+        "days",
+        "90th percentile of root zone residence time",
+        time_dependent=True,
+        active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
+    ),
     "rtavg_rz": Variable(
         "average of root zone residence time",
         CATCH_GRID,
         "days",
         "average of root zone residence time",
         time_dependent=True,
         active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
@@ -2522,14 +2552,22 @@
         CATCH_GRID + TIMESTEPS,
         "per mil",
         "isotope ratio of subsoil",
         time_dependent=True,
         write_to_restart=True,
         active=lambda settings: settings.enable_offline_transport & (settings.enable_oxygen18 | settings.enable_deuterium),
     ),
+    "rt10_ss": Variable(
+        "10th percentile of subsoil residence time",
+        CATCH_GRID,
+        "days",
+        "10th percentile of subsoil residence time",
+        time_dependent=True,
+        active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
+    ),
     "rt25_ss": Variable(
         "25th percentile of subsoil residence time",
         CATCH_GRID,
         "days",
         "25th percentile of subsoil residence time",
         time_dependent=True,
         active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
@@ -2546,14 +2584,22 @@
         "75th percentile of subsoil residence time",
         CATCH_GRID,
         "days",
         "75th percentile of subsoil residence time",
         time_dependent=True,
         active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
     ),
+    "rt90_ss": Variable(
+        "90th percentile of subsoil residence time",
+        CATCH_GRID,
+        "days",
+        "90th percentile of subsoil residence time",
+        time_dependent=True,
+        active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
+    ),
     "rtavg_ss": Variable(
         "average of subsoil residence time",
         CATCH_GRID,
         "days",
         "average of subsoil residence time",
         time_dependent=True,
         active=lambda settings: settings.enable_offline_transport & settings.enable_age_statistics,
@@ -3902,14 +3948,22 @@
         "redistribution after root loss",
         CATCH_GRID,
         "mm/dt",
         "redistribution after root loss",
         time_dependent=True,
         active=lambda settings: settings.enable_crop_phenology,
     ),
+    "re_rl_pwp": Variable(
+        "redistribution of immobile soil water after root loss",
+        CATCH_GRID,
+        "mm/dt",
+        "redistribution of immobile soil water after root loss",
+        time_dependent=True,
+        active=lambda settings: settings.enable_crop_phenology,
+    ),
     "sas_params_re_rl": Variable(
         "SAS parameters of redistribution after root loss",
         CATCH_GRID + N_SAS_PARAMS,
         "-",
         "SAS parameters of redistribution after root loss",
         time_dependent=True,
         write_to_restart=True,
@@ -4198,14 +4252,22 @@
         "redistribution after root growth",
         CATCH_GRID,
         "mm/dt",
         "redistribution after root growth",
         time_dependent=True,
         active=lambda settings: settings.enable_crop_phenology,
     ),
+    "re_rg_pwp": Variable(
+        "redistribution of immobile soil water after root growth",
+        CATCH_GRID,
+        "mm/dt",
+        "redistribution of immobile soil water after root growth",
+        time_dependent=True,
+        active=lambda settings: settings.enable_crop_phenology,
+    ),
     "sas_params_re_rg": Variable(
         "SAS parameters of redistribution after root growth",
         CATCH_GRID + N_SAS_PARAMS,
         "-",
         "SAS parameters of redistribution after root growth",
         time_dependent=True,
         write_to_restart=True,
@@ -4779,15 +4841,15 @@
     "C_in": Variable(
         "solute concentration of input",
         CATCH_GRID,
         "mg/l or per mil",
         "solute concentration of input",
         write_to_restart=False,
         time_dependent=False,
-        active=lambda settings: settings.enable_offline_transport & (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate),
+        active=lambda settings: settings.enable_offline_transport & (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer),
     ),
     "C_iso_in": Variable(
         "isotope ratio of input",
         CATCH_GRID,
         "per mil",
         "isotope ratio of input",
         write_to_restart=False,
@@ -4833,15 +4895,15 @@
     "M_in": Variable(
         "solute mass of input",
         CATCH_GRID,
         "mg",
         "solute mass of input",
         write_to_restart=False,
         time_dependent=False,
-        active=lambda settings: settings.enable_offline_transport & (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate),
+        active=lambda settings: settings.enable_offline_transport & (settings.enable_chloride | settings.enable_bromide | settings.enable_oxygen18 | settings.enable_deuterium | settings.enable_nitrate | settings.enable_virtualtracer),
     ),
     "NMIN_IN": Variable(
         "mineral nitrogen fertilizer",
         CATCH_GRID + TIME,
         "mg",
         "mineral nitrogen fertilizer",
         write_to_restart=True,
@@ -5160,14 +5222,34 @@
         "-",
         "scaling factor of crop parameters",
         write_to_restart=True,
         initial=1,
         time_dependent=False,
         active=lambda settings: not settings.enable_offline_transport and settings.enable_crop_phenology,
     ),
+    "root_growth_scale": Variable(
+        "scaling factor of crop root growth parameters",
+        CATCH_GRID,
+        "-",
+        "scaling factor of crop root growth parameters",
+        write_to_restart=True,
+        initial=1,
+        time_dependent=False,
+        active=lambda settings: not settings.enable_offline_transport and settings.enable_crop_phenology,
+    ),
+    "canopy_growth_scale": Variable(
+        "scaling factor of crop canopy growth parameters",
+        CATCH_GRID,
+        "-",
+        "scaling factor of crop canopy growth parameters",
+        write_to_restart=True,
+        initial=1,
+        time_dependent=False,
+        active=lambda settings: not settings.enable_offline_transport and settings.enable_crop_phenology,
+    ),
     "lut_crop_scale": Variable(
         "scaling factor of crop parameters",
         CATCH_GRID + N_CROP_TYPES,
         "-",
         "scaling factor of crop parameters",
         write_to_restart=True,
         initial=1,
@@ -5301,22 +5383,56 @@
         "numerical error of water balance",
         CATCH_GRID,
         "mm",
         "numerical error of water balance",
         write_to_restart=False,
         time_dependent=False,
     ),
+    "dS_rz_num_error": Variable(
+        "numerical error of root zone water balance",
+        CATCH_GRID,
+        "mm",
+        "numerical error of root zone water balance",
+        write_to_restart=False,
+        time_dependent=False,
+    ),
+    "dS_ss_num_error": Variable(
+        "numerical error of subsoil water balance",
+        CATCH_GRID,
+        "mm",
+        "numerical error of subsoil water balance",
+        write_to_restart=False,
+        time_dependent=False,
+    ),
     "dC_num_error": Variable(
         "numerical error of solute balance",
         CATCH_GRID,
         "M",
         "numerical error of solute balance",
         write_to_restart=False,
         time_dependent=False,
         active=lambda settings: settings.enable_offline_transport,
+    ),
+    "dC_rz_num_error": Variable(
+        "numerical error of solute balance",
+        CATCH_GRID,
+        "M",
+        "numerical error of solute balance",
+        write_to_restart=False,
+        time_dependent=False,
+        active=lambda settings: settings.enable_offline_transport,
+    ),
+    "dC_ss_num_error": Variable(
+        "numerical error of solute balance",
+        CATCH_GRID,
+        "M",
+        "numerical error of solute balance",
+        write_to_restart=False,
+        time_dependent=False,
+        active=lambda settings: settings.enable_offline_transport,
     ),
 }
 
 
 def manifest_metadata(var_meta, settings):
     """Evaluate callable metadata fields given the current settings."""
     from copy import copy
```

### Comparing `roger-3.0/roger.egg-info/PKG-INFO` & `roger-3.0.1/roger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roger
-Version: 3.0
+Version: 3.0.1
 Summary: Runoff Generation Research - a hydrologic toolbox in Python
 Home-page: https://roger.readthedocs.io
 Author: Robin Schwemmle (University of Freiburg)
 Author-email: robin.schwemmle@hydrology.uni-freiburg.de
 License: MIT
 Keywords: hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax
 Classifier: Development Status :: 4 - Beta
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 <p align="center">
 <img src="doc/_images/roger-logo.png">
 </p>
 
 <p align="center">
-<i>Runoff Generation Research - a hydrologic toolbox in Python</i>
+<i>Runoff Generation Research - a process-based hydrological toolbox model in Python</i>
 </p>
 
 <p align="center">
   <a href="http://roger.readthedocs.io/?badge=latest">
     <img src="https://readthedocs.org/projects/roger/badge/?version=latest" alt="Documentation status">
   </a>
   <a href="https://github.com/Hydrology-IFH/roger/actions/workflows/test-all.yml">
@@ -43,17 +43,17 @@
   </a>
   <a href="https://codecov.io/gh/Hydrology-IFH/roger" > 
   <img src="https://codecov.io/gh/Hydrology-IFH/roger/branch/main/graph/badge.svg?token=KXSVNGDDNH"/> 
   </a>
   <a href="https://zenodo.org/badge/latestdoi/536477819"><img src="https://zenodo.org/badge/536477819.svg" alt="DOI"></a>
 </p>
 
-Roger, *Runoff Generation Research*, is a process-based hydrologic model that can be applied from plot to catchment scale. Roger is written in pure Python, which facilitates model setup and model workflows. We want to enable high-performance hydrologic modelling with a clear focus on flexibility and usability.
+RoGeR, *Runoff Generation Research*, is a process-based hydrological model that can be applied from plot to catchment scale. RoGeR is written in pure Python, which facilitates model setup and model workflows. We want to enable high-performance hydrologic modelling with a clear focus on flexibility and usability.
 
-Roger supports a NumPy backend for small-scale problems, and a
+RoGeR supports a NumPy backend for small-scale problems, and a
 high-performance [JAX](https://github.com/google/jax) backend
 with CPU and GPU support. Parallel computation is available via MPI and supports
 distributed execution on any number of nodes/CPU cores.
 
 Inspired by [Veros](https://veros.readthedocs.io/en/latest/).
 
 ## Documentation
@@ -136,15 +136,15 @@
 
 ## How to cite
 
 If you use Roger in scientific work, please consider citing [the following publication](...):
 
 ```bibtex
 @article{
-	title = {Roger v3.0 – a hydrologic toolbox in {Python}},
+	title = {Roger v3.0 – a process-based hydrologic toolbox model in {Python}},
 	volume = {...},
 	doi = {https://doi.org/10.5194/gmd-xxx},
 	journal = {Geosci. Model Dev.},
 	author = {Schwemmle, Robin, and Leistert, Hannes, and Weiler, Markus},
 	year = {2023},
 	pages = {...},
 }
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roger Version: 3.0 Summary: Runoff Generation
+Metadata-Version: 2.1 Name: roger Version: 3.0.1 Summary: Runoff Generation
 Research - a hydrologic toolbox in Python Home-page: https://
 roger.readthedocs.io Author: Robin Schwemmle (University of Freiburg) Author-
 email: robin.schwemmle@hydrology.uni-freiburg.de License: MIT Keywords:
 hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -10,22 +10,23 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX Classifier: Operating System :: Unix Classifier: Operating
 System :: MacOS Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: test Provides-Extra: jax License-File: LICENSE
                          [doc/_images/roger-logo.png]
-          Runoff Generation Research - a hydrologic toolbox in Python
+  Runoff Generation Research - a process-based hydrological toolbox model in
+                                    Python
   [Documentation_status] [Test_status] [https://codecov.io/gh/Hydrology-IFH/
            roger/branch/main/graph/badge.svg?token=KXSVNGDDNH] [DOI]
-Roger, *Runoff Generation Research*, is a process-based hydrologic model that
-can be applied from plot to catchment scale. Roger is written in pure Python,
+RoGeR, *Runoff Generation Research*, is a process-based hydrological model that
+can be applied from plot to catchment scale. RoGeR is written in pure Python,
 which facilitates model setup and model workflows. We want to enable high-
 performance hydrologic modelling with a clear focus on flexibility and
-usability. Roger supports a NumPy backend for small-scale problems, and a high-
+usability. RoGeR supports a NumPy backend for small-scale problems, and a high-
 performance [JAX](https://github.com/google/jax) backend with CPU and GPU
 support. Parallel computation is available via MPI and supports distributed
 execution on any number of nodes/CPU cores. Inspired by [Veros](https://
 veros.readthedocs.io/en/latest/). ## Documentation We strongly recommend to
 [visit our documentation](https://roger.readthedocs.io/en/latest/). ## Features
                     [25_square_meter_resolved_simulations_
                     of_a_rectangular_soil_covered_by_grass]
@@ -62,23 +63,23 @@
 some tips on testing and benchmarking, and to make sure that your modifications
 adhere with our style policies. Most importantly, please ensure that you follow
 the [PEP8 guidelines](https://www.python.org/dev/peps/pep-0008/), use
 *meaningful* variable names, and document your code using [Google-style
 docstrings](http://sphinxcontrib-napoleon.readthedocs.io/en/latest/
 example_google.html). ## How to cite If you use Roger in scientific work,
 please consider citing [the following publication](...): ```bibtex @article
-{ title = {Roger v3.0 â a hydrologic toolbox in {Python}}, volume = {...},
-doi = {https://doi.org/10.5194/gmd-xxx}, journal = {Geosci. Model Dev.}, author
-= {Schwemmle, Robin, and Leistert, Hannes, and Weiler, Markus}, year = {2023},
-pages = {...}, } ``` Or have a look at [our documentation](https://
-roger.readthedocs.io/en/latest/more/publications.html) for more publications
-involving Roger. ## TODO - implement runoff and channel routing (e.g. kinematic
-wave or hydraulic approach) - implement distributed model with run-on
-infiltration - use coarser spatial and temporal resolution for computation of
-groundwater-related processes - implement baseflow in the groundwater routine.
-requires surface water depth. - implement surface runoff generation for
-gravity-driven infiltration - implement gravity-driven infiltration and
-percolation and include it into the transport routine - implement time-variant
-sowing and harvesting of crops ## License This software can be distributed
-freely under the MIT license. Please read the LICENSE for further information.
-Â© 2022, Robin Schwemmle (
+{ title = {Roger v3.0 â a process-based hydrologic toolbox model in
+{Python}}, volume = {...}, doi = {https://doi.org/10.5194/gmd-xxx}, journal =
+{Geosci. Model Dev.}, author = {Schwemmle, Robin, and Leistert, Hannes, and
+Weiler, Markus}, year = {2023}, pages = {...}, } ``` Or have a look at [our
+documentation](https://roger.readthedocs.io/en/latest/more/publications.html)
+for more publications involving Roger. ## TODO - implement runoff and channel
+routing (e.g. kinematic wave or hydraulic approach) - implement distributed
+model with run-on infiltration - use coarser spatial and temporal resolution
+for computation of groundwater-related processes - implement baseflow in the
+groundwater routine. requires surface water depth. - implement surface runoff
+generation for gravity-driven infiltration - implement gravity-driven
+infiltration and percolation and include it into the transport routine -
+implement time-variant sowing and harvesting of crops ## License This software
+can be distributed freely under the MIT license. Please read the LICENSE for
+further information. Â© 2022, Robin Schwemmle (
 schwemmle@hydrology.uni-freiburg.de>)
```

### Comparing `roger-3.0/roger.egg-info/SOURCES.txt` & `roger-3.0.1/roger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roger-3.0/setup.py` & `roger-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/test/cli_test.py` & `roger-3.0.1/test/cli_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/test/make_data_for_svat_transport.py` & `roger-3.0.1/test/make_data_for_svat_transport.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/test/progress_test.py` & `roger-3.0.1/test/progress_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import sys
-import re
 import time
 import platform
-
 import pytest
 
 
 class Dummy:
     pass
```

### Comparing `roger-3.0/test/restart_test.py` & `roger-3.0.1/test/restart_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/test/setup_test.py` & `roger-3.0.1/test/setup_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/test/state_test.py` & `roger-3.0.1/test/state_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0/versioneer.py` & `roger-3.0.1/versioneer.py`

 * *Files identical despite different names*

