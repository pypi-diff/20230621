# Comparing `tmp/roger-0.1.2.tar.gz` & `tmp/roger-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roger-0.1.2.tar", last modified: Fri Feb 10 15:46:18 2023, max compression
+gzip compressed data, was "roger-3.0.tar", last modified: Sun Feb 12 14:19:42 2023, max compression
```

## Comparing `roger-0.1.2.tar` & `roger-3.0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.105670 roger-0.1.2/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1072 2023-01-28 18:10:37.000000 roger-0.1.2/LICENSE
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      521 2023-02-10 12:04:56.000000 roger-0.1.2/MANIFEST.in
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    10871 2023-02-10 15:46:18.105906 roger-0.1.2/PKG-INFO
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     9773 2023-02-08 18:35:56.000000 roger-0.1.2/README.md
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4083 2023-01-28 18:10:37.000000 roger-0.1.2/cuda_ext.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:17.989265 roger-0.1.2/look_up_tables/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     9303 2023-01-28 18:10:43.000000 roger-0.1.2/look_up_tables/crop_parameters.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     1174 2023-01-28 18:10:43.000000 roger-0.1.2/look_up_tables/intercept_land_use.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      818 2023-01-28 18:10:43.000000 roger-0.1.2/look_up_tables/intercept_sealing.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     3122 2023-01-28 18:10:43.000000 roger-0.1.2/look_up_tables/mp_drain_area.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)   587663 2023-01-28 18:10:43.000000 roger-0.1.2/look_up_tables/mp_layer_manning_strickler.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      672 2023-01-28 18:10:43.000000 roger-0.1.2/look_up_tables/root_depth_land_use.csv
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      247 2023-01-28 18:10:43.000000 roger-0.1.2/pyproject.toml
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      186 2023-02-10 15:42:45.000000 roger-0.1.2/requirements.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       27 2023-02-08 17:52:32.000000 roger-0.1.2/requirements_jax.txt
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.107183 roger-0.1.2/roger/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2354 2023-01-28 18:10:43.000000 roger-0.1.2/roger/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      497 2023-02-10 15:46:18.107341 roger-0.1.2/roger/_version.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2410 2023-01-28 18:10:43.000000 roger-0.1.2/roger/backend.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.026358 roger-0.1.2/roger/cli/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      584 2023-01-28 18:10:43.000000 roger-0.1.2/roger/cli/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      116 2023-01-28 18:10:43.000000 roger-0.1.2/roger/cli/roger.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3143 2023-01-28 18:10:43.000000 roger-0.1.2/roger/cli/roger_copy_model.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1045 2023-01-28 18:10:43.000000 roger-0.1.2/roger/cli/roger_create_mask.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3066 2023-01-28 18:10:43.000000 roger-0.1.2/roger/cli/roger_resubmit.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4344 2023-01-28 18:10:43.000000 roger-0.1.2/roger/cli/roger_run.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1410 2023-01-28 18:10:43.000000 roger-0.1.2/roger/cli/roger_run_base.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.059743 roger-0.1.2/roger/core/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1364 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    21126 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/adaptive_time_stepping.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    17885 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/capillary_rise.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    66629 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/crop.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    26780 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/evapotranspiration.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    23142 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/film_flow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4075 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/groundwater.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3592 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/groundwater_flow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    69882 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/infiltration.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13502 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/interception.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     9290 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/nitrate.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    26889 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/numerics.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5705 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/operators.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7632 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/root_zone.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11373 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/sas.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11056 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/snow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    46149 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/soil.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7656 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/subsoil.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    58575 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/subsurface_runoff.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13121 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/surface.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      258 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/surface_runoff.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)   170691 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/transport.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4838 2023-01-28 18:10:43.000000 roger-0.1.2/roger/core/utilities.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.071124 roger-0.1.2/roger/diagnostics/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      105 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2059 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/api.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3307 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/average.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4047 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/base.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2756 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/collect.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2790 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/constant.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3793 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/maximum.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3794 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/minimum.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2839 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/rate.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1580 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/snapshot.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1360 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/tracer_monitor.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1378 2023-01-28 18:10:43.000000 roger-0.1.2/roger/diagnostics/water_monitor.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    18158 2023-01-28 18:10:43.000000 roger-0.1.2/roger/distributed.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.074856 roger-0.1.2/roger/io_tools/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-0.1.2/roger/io_tools/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6124 2023-01-28 18:10:43.000000 roger-0.1.2/roger/io_tools/csv.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1660 2023-01-28 18:10:43.000000 roger-0.1.2/roger/io_tools/hdf5.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6257 2023-01-28 18:10:43.000000 roger-0.1.2/roger/io_tools/netcdf.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      522 2023-01-28 18:10:43.000000 roger-0.1.2/roger/io_tools/yml.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1907 2023-01-28 18:10:43.000000 roger-0.1.2/roger/logs.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2576 2023-01-28 18:10:43.000000 roger-0.1.2/roger/lookuptables.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.075573 roger-0.1.2/roger/models/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/__init__.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.076721 roger-0.1.2/roger/models/dummy/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/dummy/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1251 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/dummy/dummy.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.078338 roger-0.1.2/roger/models/oneD/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/oneD/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13312 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/oneD/oneD.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.080073 roger-0.1.2/roger/models/oneD_event/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       76 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/oneD_event/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11459 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/oneD_event/oneD_event.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.082151 roger-0.1.2/roger/models/svat/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11572 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat/svat.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.083805 roger-0.1.2/roger/models/svat_bromide/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       84 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_bromide/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14478 2023-02-08 16:26:37.000000 roger-0.1.2/roger/models/svat_bromide/svat_bromide.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.085881 roger-0.1.2/roger/models/svat_crop/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       73 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_crop/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    16051 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_crop/svat_crop.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.087855 roger-0.1.2/roger/models/svat_crop_bromide/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_crop_bromide/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_crop_bromide/svat_crop_bromide.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.089215 roger-0.1.2/roger/models/svat_crop_nitrate/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_crop_nitrate/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_crop_nitrate/svat_crop_nitrate.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.090530 roger-0.1.2/roger/models/svat_oxygen18/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       86 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_oxygen18/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    19035 2023-01-28 18:10:43.000000 roger-0.1.2/roger/models/svat_oxygen18/svat_oxygen18.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1936 2023-01-28 18:10:43.000000 roger-0.1.2/roger/plugins.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6475 2023-01-28 18:10:43.000000 roger-0.1.2/roger/progress.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6221 2023-01-28 18:10:43.000000 roger-0.1.2/roger/restart.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    25023 2023-01-28 18:10:43.000000 roger-0.1.2/roger/roger.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14190 2023-01-28 18:10:43.000000 roger-0.1.2/roger/routines.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5954 2023-01-28 18:10:43.000000 roger-0.1.2/roger/runtime.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     9199 2023-01-28 18:10:43.000000 roger-0.1.2/roger/settings.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2330 2023-01-28 18:10:43.000000 roger-0.1.2/roger/signals.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    17650 2023-01-28 18:10:43.000000 roger-0.1.2/roger/state.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      819 2023-01-28 18:10:43.000000 roger-0.1.2/roger/time.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      451 2023-01-28 18:10:43.000000 roger-0.1.2/roger/timer.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.097557 roger-0.1.2/roger/tools/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-0.1.2/roger/tools/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    31909 2023-01-28 18:10:43.000000 roger-0.1.2/roger/tools/evaluation.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    20672 2023-01-28 18:10:43.000000 roger-0.1.2/roger/tools/event_classification.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    12678 2023-01-28 18:10:43.000000 roger-0.1.2/roger/tools/filelock.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14559 2023-01-28 18:10:43.000000 roger-0.1.2/roger/tools/labels.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    24578 2023-01-28 18:10:43.000000 roger-0.1.2/roger/tools/make_toy_data.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      134 2023-01-28 18:10:43.000000 roger-0.1.2/roger/tools/plotting.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    22516 2023-01-28 18:10:43.000000 roger-0.1.2/roger/tools/setup.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)   176931 2023-01-28 18:10:43.000000 roger-0.1.2/roger/variables.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.020060 roger-0.1.2/roger.egg-info/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    10871 2023-02-10 15:46:16.000000 roger-0.1.2/roger.egg-info/PKG-INFO
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3170 2023-02-10 15:46:17.000000 roger-0.1.2/roger.egg-info/SOURCES.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2023-02-10 15:46:16.000000 roger-0.1.2/roger.egg-info/dependency_links.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      270 2023-02-10 15:46:16.000000 roger-0.1.2/roger.egg-info/entry_points.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2023-02-10 15:15:06.000000 roger-0.1.2/roger.egg-info/not-zip-safe
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      291 2023-02-10 15:46:16.000000 roger-0.1.2/roger.egg-info/requires.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       11 2023-02-10 15:46:16.000000 roger-0.1.2/roger.egg-info/top_level.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      327 2023-02-10 15:46:18.106752 roger-0.1.2/setup.cfg
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4609 2023-01-28 18:10:43.000000 roger-0.1.2/setup.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-10 15:46:18.105021 roger-0.1.2/test/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      103 2023-02-08 16:07:16.000000 roger-0.1.2/test/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1075 2023-01-28 18:10:43.000000 roger-0.1.2/test/cli_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      391 2023-02-08 13:33:29.000000 roger-0.1.2/test/conftest.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    23321 2023-02-08 17:11:16.000000 roger-0.1.2/test/make_data_for_svat_transport.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1076 2023-02-08 18:10:29.000000 roger-0.1.2/test/progress_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2684 2023-01-28 18:10:43.000000 roger-0.1.2/test/restart_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5047 2023-02-08 17:11:11.000000 roger-0.1.2/test/setup_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3320 2023-02-08 13:27:57.000000 roger-0.1.2/test/state_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    68611 2023-01-28 18:10:43.000000 roger-0.1.2/versioneer.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.705093 roger-3.0/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1072 2023-01-28 18:10:37.000000 roger-3.0/LICENSE
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      521 2023-02-10 12:04:56.000000 roger-3.0/MANIFEST.in
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6978 2023-02-12 14:19:42.706682 roger-3.0/PKG-INFO
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5864 2023-02-10 20:42:33.000000 roger-3.0/README.md
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4083 2023-01-28 18:10:37.000000 roger-3.0/cuda_ext.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.487710 roger-3.0/look_up_tables/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     9303 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/crop_parameters.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     1174 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/intercept_land_use.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      818 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/intercept_sealing.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     3122 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/mp_drain_area.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)   587663 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/mp_layer_manning_strickler.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      672 2023-01-28 18:10:43.000000 roger-3.0/look_up_tables/root_depth_land_use.csv
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      247 2023-01-28 18:10:43.000000 roger-3.0/pyproject.toml
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      186 2023-02-10 15:42:45.000000 roger-3.0/requirements.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       27 2023-02-08 17:52:32.000000 roger-3.0/requirements_jax.txt
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.739269 roger-3.0/roger/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2354 2023-01-28 18:10:43.000000 roger-3.0/roger/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      495 2023-02-12 14:19:42.739524 roger-3.0/roger/_version.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2410 2023-01-28 18:10:43.000000 roger-3.0/roger/backend.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.532441 roger-3.0/roger/cli/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      584 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      116 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3143 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_copy_model.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1045 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_create_mask.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3066 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_resubmit.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4344 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_run.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1410 2023-01-28 18:10:43.000000 roger-3.0/roger/cli/roger_run_base.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.563441 roger-3.0/roger/core/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1364 2023-01-28 18:10:43.000000 roger-3.0/roger/core/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    21126 2023-01-28 18:10:43.000000 roger-3.0/roger/core/adaptive_time_stepping.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    17885 2023-01-28 18:10:43.000000 roger-3.0/roger/core/capillary_rise.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    66629 2023-01-28 18:10:43.000000 roger-3.0/roger/core/crop.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    26780 2023-01-28 18:10:43.000000 roger-3.0/roger/core/evapotranspiration.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    23142 2023-01-28 18:10:43.000000 roger-3.0/roger/core/film_flow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4075 2023-01-28 18:10:43.000000 roger-3.0/roger/core/groundwater.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3592 2023-01-28 18:10:43.000000 roger-3.0/roger/core/groundwater_flow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    69882 2023-01-28 18:10:43.000000 roger-3.0/roger/core/infiltration.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13502 2023-01-28 18:10:43.000000 roger-3.0/roger/core/interception.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     9290 2023-01-28 18:10:43.000000 roger-3.0/roger/core/nitrate.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    26889 2023-01-28 18:10:43.000000 roger-3.0/roger/core/numerics.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5705 2023-01-28 18:10:43.000000 roger-3.0/roger/core/operators.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7632 2023-01-28 18:10:43.000000 roger-3.0/roger/core/root_zone.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11373 2023-01-28 18:10:43.000000 roger-3.0/roger/core/sas.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11056 2023-01-28 18:10:43.000000 roger-3.0/roger/core/snow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    46149 2023-01-28 18:10:43.000000 roger-3.0/roger/core/soil.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7656 2023-01-28 18:10:43.000000 roger-3.0/roger/core/subsoil.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    58575 2023-01-28 18:10:43.000000 roger-3.0/roger/core/subsurface_runoff.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13121 2023-01-28 18:10:43.000000 roger-3.0/roger/core/surface.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      258 2023-01-28 18:10:43.000000 roger-3.0/roger/core/surface_runoff.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)   170691 2023-01-28 18:10:43.000000 roger-3.0/roger/core/transport.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4838 2023-01-28 18:10:43.000000 roger-3.0/roger/core/utilities.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.575245 roger-3.0/roger/diagnostics/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      105 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2059 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/api.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3307 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/average.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4047 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/base.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2756 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/collect.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2790 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/constant.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3793 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/maximum.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3794 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/minimum.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2839 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/rate.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1580 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/snapshot.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1360 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/tracer_monitor.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1378 2023-01-28 18:10:43.000000 roger-3.0/roger/diagnostics/water_monitor.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    18158 2023-01-28 18:10:43.000000 roger-3.0/roger/distributed.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.582122 roger-3.0/roger/io_tools/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6124 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/csv.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1660 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/hdf5.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6257 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/netcdf.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      522 2023-01-28 18:10:43.000000 roger-3.0/roger/io_tools/yml.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1907 2023-01-28 18:10:43.000000 roger-3.0/roger/logs.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2576 2023-01-28 18:10:43.000000 roger-3.0/roger/lookuptables.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.583876 roger-3.0/roger/models/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/models/__init__.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.585542 roger-3.0/roger/models/dummy/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-01-28 18:10:43.000000 roger-3.0/roger/models/dummy/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1251 2023-01-28 18:10:43.000000 roger-3.0/roger/models/dummy/dummy.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.590098 roger-3.0/roger/models/oneD/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0/roger/models/oneD/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13312 2023-01-28 18:10:43.000000 roger-3.0/roger/models/oneD/oneD.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.593186 roger-3.0/roger/models/oneD_event/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       76 2023-01-28 18:10:43.000000 roger-3.0/roger/models/oneD_event/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11459 2023-01-28 18:10:43.000000 roger-3.0/roger/models/oneD_event/oneD_event.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.595985 roger-3.0/roger/models/svat/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11572 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat/svat.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.600371 roger-3.0/roger/models/svat_bromide/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       84 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_bromide/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14478 2023-02-08 16:26:37.000000 roger-3.0/roger/models/svat_bromide/svat_bromide.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.604427 roger-3.0/roger/models/svat_crop/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       73 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    16051 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop/svat_crop.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.607837 roger-3.0/roger/models/svat_crop_bromide/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop_bromide/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop_bromide/svat_crop_bromide.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.611148 roger-3.0/roger/models/svat_crop_nitrate/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop_nitrate/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_crop_nitrate/svat_crop_nitrate.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.613200 roger-3.0/roger/models/svat_oxygen18/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       86 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_oxygen18/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    19035 2023-01-28 18:10:43.000000 roger-3.0/roger/models/svat_oxygen18/svat_oxygen18.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1936 2023-01-28 18:10:43.000000 roger-3.0/roger/plugins.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6475 2023-01-28 18:10:43.000000 roger-3.0/roger/progress.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6221 2023-01-28 18:10:43.000000 roger-3.0/roger/restart.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    25023 2023-01-28 18:10:43.000000 roger-3.0/roger/roger.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14190 2023-01-28 18:10:43.000000 roger-3.0/roger/routines.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5954 2023-01-28 18:10:43.000000 roger-3.0/roger/runtime.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     9218 2023-02-11 12:18:32.000000 roger-3.0/roger/settings.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2330 2023-01-28 18:10:43.000000 roger-3.0/roger/signals.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    17650 2023-01-28 18:10:43.000000 roger-3.0/roger/state.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      819 2023-01-28 18:10:43.000000 roger-3.0/roger/time.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      451 2023-01-28 18:10:43.000000 roger-3.0/roger/timer.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.630768 roger-3.0/roger/tools/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    31909 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/evaluation.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    20672 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/event_classification.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    12678 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/filelock.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14559 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/labels.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    24578 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/make_toy_data.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      134 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/plotting.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    22516 2023-01-28 18:10:43.000000 roger-3.0/roger/tools/setup.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)   176931 2023-01-28 18:10:43.000000 roger-3.0/roger/variables.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.525638 roger-3.0/roger.egg-info/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6978 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/PKG-INFO
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3170 2023-02-12 14:19:42.000000 roger-3.0/roger.egg-info/SOURCES.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/dependency_links.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      270 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/entry_points.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2023-02-10 15:15:06.000000 roger-3.0/roger.egg-info/not-zip-safe
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      291 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/requires.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       11 2023-02-12 14:19:39.000000 roger-3.0/roger.egg-info/top_level.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      327 2023-02-12 14:19:42.730873 roger-3.0/setup.cfg
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4627 2023-02-10 16:39:56.000000 roger-3.0/setup.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2023-02-12 14:19:42.699889 roger-3.0/test/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      103 2023-02-08 16:07:16.000000 roger-3.0/test/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1075 2023-01-28 18:10:43.000000 roger-3.0/test/cli_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      391 2023-02-08 13:33:29.000000 roger-3.0/test/conftest.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    23321 2023-02-08 17:11:16.000000 roger-3.0/test/make_data_for_svat_transport.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1076 2023-02-08 18:10:29.000000 roger-3.0/test/progress_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2684 2023-01-28 18:10:43.000000 roger-3.0/test/restart_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5047 2023-02-08 17:11:11.000000 roger-3.0/test/setup_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3320 2023-02-08 13:27:57.000000 roger-3.0/test/state_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    68611 2023-01-28 18:10:43.000000 roger-3.0/versioneer.py
```

### Comparing `roger-0.1.2/LICENSE` & `roger-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/MANIFEST.in` & `roger-3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/cuda_ext.py` & `roger-3.0/cuda_ext.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/look_up_tables/crop_parameters.csv` & `roger-3.0/look_up_tables/crop_parameters.csv`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/look_up_tables/intercept_land_use.csv` & `roger-3.0/look_up_tables/intercept_land_use.csv`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/look_up_tables/intercept_sealing.csv` & `roger-3.0/look_up_tables/intercept_sealing.csv`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/look_up_tables/mp_drain_area.csv` & `roger-3.0/look_up_tables/mp_drain_area.csv`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/look_up_tables/mp_layer_manning_strickler.csv` & `roger-3.0/look_up_tables/mp_layer_manning_strickler.csv`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/look_up_tables/root_depth_land_use.csv` & `roger-3.0/look_up_tables/root_depth_land_use.csv`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/__init__.py` & `roger-3.0/roger/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/backend.py` & `roger-3.0/roger/backend.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/cli/__init__.py` & `roger-3.0/roger/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/cli/roger_copy_model.py` & `roger-3.0/roger/cli/roger_copy_model.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/cli/roger_create_mask.py` & `roger-3.0/roger/cli/roger_create_mask.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/cli/roger_resubmit.py` & `roger-3.0/roger/cli/roger_resubmit.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/cli/roger_run.py` & `roger-3.0/roger/cli/roger_run.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/cli/roger_run_base.py` & `roger-3.0/roger/cli/roger_run_base.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/__init__.py` & `roger-3.0/roger/core/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/adaptive_time_stepping.py` & `roger-3.0/roger/core/adaptive_time_stepping.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/capillary_rise.py` & `roger-3.0/roger/core/capillary_rise.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/crop.py` & `roger-3.0/roger/core/crop.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/evapotranspiration.py` & `roger-3.0/roger/core/evapotranspiration.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/film_flow.py` & `roger-3.0/roger/core/film_flow.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/groundwater.py` & `roger-3.0/roger/core/groundwater.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/groundwater_flow.py` & `roger-3.0/roger/core/groundwater_flow.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/infiltration.py` & `roger-3.0/roger/core/infiltration.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/interception.py` & `roger-3.0/roger/core/interception.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/nitrate.py` & `roger-3.0/roger/core/nitrate.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/numerics.py` & `roger-3.0/roger/core/numerics.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/operators.py` & `roger-3.0/roger/core/operators.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/root_zone.py` & `roger-3.0/roger/core/root_zone.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/sas.py` & `roger-3.0/roger/core/sas.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/snow.py` & `roger-3.0/roger/core/snow.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/soil.py` & `roger-3.0/roger/core/soil.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/subsoil.py` & `roger-3.0/roger/core/subsoil.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/subsurface_runoff.py` & `roger-3.0/roger/core/subsurface_runoff.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/surface.py` & `roger-3.0/roger/core/surface.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/transport.py` & `roger-3.0/roger/core/transport.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/core/utilities.py` & `roger-3.0/roger/core/utilities.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/api.py` & `roger-3.0/roger/diagnostics/api.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/average.py` & `roger-3.0/roger/diagnostics/average.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/base.py` & `roger-3.0/roger/diagnostics/base.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/collect.py` & `roger-3.0/roger/diagnostics/collect.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/constant.py` & `roger-3.0/roger/diagnostics/constant.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/maximum.py` & `roger-3.0/roger/diagnostics/maximum.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/minimum.py` & `roger-3.0/roger/diagnostics/minimum.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/rate.py` & `roger-3.0/roger/diagnostics/rate.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/snapshot.py` & `roger-3.0/roger/diagnostics/snapshot.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/tracer_monitor.py` & `roger-3.0/roger/diagnostics/tracer_monitor.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/diagnostics/water_monitor.py` & `roger-3.0/roger/diagnostics/water_monitor.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/distributed.py` & `roger-3.0/roger/distributed.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/io_tools/csv.py` & `roger-3.0/roger/io_tools/csv.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/io_tools/hdf5.py` & `roger-3.0/roger/io_tools/hdf5.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/io_tools/netcdf.py` & `roger-3.0/roger/io_tools/netcdf.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/io_tools/yml.py` & `roger-3.0/roger/io_tools/yml.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/logs.py` & `roger-3.0/roger/logs.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/lookuptables.py` & `roger-3.0/roger/lookuptables.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/models/dummy/dummy.py` & `roger-3.0/roger/models/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/models/oneD/oneD.py` & `roger-3.0/roger/models/oneD/oneD.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/models/oneD_event/oneD_event.py` & `roger-3.0/roger/models/oneD_event/oneD_event.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/models/svat/svat.py` & `roger-3.0/roger/models/svat/svat.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/models/svat_bromide/svat_bromide.py` & `roger-3.0/roger/models/svat_bromide/svat_bromide.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/models/svat_crop/svat_crop.py` & `roger-3.0/roger/models/svat_crop/svat_crop.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/models/svat_oxygen18/svat_oxygen18.py` & `roger-3.0/roger/models/svat_oxygen18/svat_oxygen18.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/plugins.py` & `roger-3.0/roger/plugins.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/progress.py` & `roger-3.0/roger/progress.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/restart.py` & `roger-3.0/roger/restart.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/roger.py` & `roger-3.0/roger/roger.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/routines.py` & `roger-3.0/roger/routines.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/runtime.py` & `roger-3.0/roger/runtime.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/settings.py` & `roger-3.0/roger/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "dt_tracer": Setting(24.0, float, "Time step for tracers, can be larger than dt"),
     "runlen": Setting(0.0, float, "Length of simulation in seconds"),
     "runlen_warmup": Setting(0.0, float, "Length of warmup simulation in seconds"),
     "x_origin": Setting(0, float, "Grid origin in x-direction"),
     "y_origin": Setting(0, float, "Grid origin in y-direction"),
     "time_origin": Setting("1900-01-01 00:00:00", str, "time origin"),
     "AB_eps": Setting(0.1, float, "Deviation from Adam-Bashforth weighting"),
-    "nsas": Setting(8, int, "Grid points of array containing SAS parameters"),
+    "nsas": Setting(8, int, "Number of entries per grid cell containing SAS parameters"),
     # Physical constants
     "pi": Setting(PI, float, "Pi"),
     "r_mp": Setting(2.5, float, "Macropore radius in mm"),
     "l_sc": Setting(10000, float, "Total length of shrinkage cracks in mm/m^2"),
     "sf": Setting(3, float, "Degree-day factor in -"),
     "ta_fm": Setting(0, float, "freeze-melt threshold in degC"),
     "rmax": Setting(30, float, "Retention capacity of liquid water in snow cover in %"),
@@ -65,19 +65,19 @@
     "rew_max": Setting(12, float, "maximum readily evaporable water in mm"),
     "z_evap_max": Setting(150, float, "maximum soil evaporation depth in mm"),
     "transp_water_stress": Setting(0.75, float, "fraction of fine pore storage in -"),
     "ccc_decay_rate": Setting(0.005, float, "decay rate of crop canopy cover in -"),
     "basal_crop_coeff_min": Setting(0.15, float, "minimum basal crop coeffcient in -"),
     "ff_tc": Setting(0.15, float, "film flow termination criterium in -"),
     "VSMOW_conc18O": Setting(2005.2e-6, float, "oxygen-18 abundancy ratios according to VSMOW in -"),
-    "d18O_min": Setting(-20, float, "potentially lowest oxygen-18 value in per mil"),
-    "d18O_max": Setting(0, float, "potentially greatest oxygen-18 value in per mil"),
+    "d18O_min": Setting(-20, float, "potentially lowest oxygen-18 value in per mille"),
+    "d18O_max": Setting(0, float, "potentially greatest oxygen-18 value in per mille"),
     "VSMOW_conc2H": Setting(155.76e-6, float, "deuterium abundancy ratios according to VSMOW in -"),
-    "d2H_min": Setting(-160, float, "potentially lowest deuterium value in per mil"),
-    "d2H_max": Setting(0, float, "potentially greatest deuterium value in per mil"),
+    "d2H_min": Setting(-160, float, "potentially lowest deuterium value in per mille"),
+    "d2H_max": Setting(0, float, "potentially greatest deuterium value in per mille"),
     # Logical switches for general model setup
     "coord_degree": Setting(False, bool, "either spherical (True) or cartesian (False) coordinates"),
     "enable_distributed_input": Setting(False, bool, "enable distributed input"),
     "enable_film_flow": Setting(False, bool, "enable film flow process"),
     "enable_lateral_flow": Setting(False, bool, "enable lateral flow"),
     "enable_crop_phenology": Setting(False, bool, "enable crop phenology"),
     "enable_crop_rotation": Setting(False, bool, "enable crop rotation"),
```

### Comparing `roger-0.1.2/roger/signals.py` & `roger-3.0/roger/signals.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/state.py` & `roger-3.0/roger/state.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/time.py` & `roger-3.0/roger/time.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/tools/evaluation.py` & `roger-3.0/roger/tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/tools/event_classification.py` & `roger-3.0/roger/tools/event_classification.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/tools/filelock.py` & `roger-3.0/roger/tools/filelock.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/tools/labels.py` & `roger-3.0/roger/tools/labels.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/tools/make_toy_data.py` & `roger-3.0/roger/tools/make_toy_data.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/tools/setup.py` & `roger-3.0/roger/tools/setup.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger/variables.py` & `roger-3.0/roger/variables.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/roger.egg-info/SOURCES.txt` & `roger-3.0/roger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/setup.py` & `roger-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
 setup(
     name="roger",
     license="MIT",
     author="Robin Schwemmle (University of Freiburg)",
     author_email="robin.schwemmle@hydrology.uni-freiburg.de",
     keywords="hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax",
-    description="Runoff Generation Research in Pure Python",
+    description="Runoff Generation Research - a hydrologic toolbox in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://roger.readthedocs.io",
     python_requires=">=3.7",
     version=versioneer.get_version(),
     cmdclass=cmdclass,
     packages=find_packages(),
```

### Comparing `roger-0.1.2/test/cli_test.py` & `roger-3.0/test/cli_test.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/test/make_data_for_svat_transport.py` & `roger-3.0/test/make_data_for_svat_transport.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/test/progress_test.py` & `roger-3.0/test/progress_test.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/test/restart_test.py` & `roger-3.0/test/restart_test.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/test/setup_test.py` & `roger-3.0/test/setup_test.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/test/state_test.py` & `roger-3.0/test/state_test.py`

 * *Files identical despite different names*

### Comparing `roger-0.1.2/versioneer.py` & `roger-3.0/versioneer.py`

 * *Files identical despite different names*

