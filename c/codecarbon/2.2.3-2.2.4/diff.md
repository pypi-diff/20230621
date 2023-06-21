# Comparing `tmp/codecarbon-2.2.3.tar.gz` & `tmp/codecarbon-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecarbon-2.2.3.tar", last modified: Mon Jun  5 05:26:02 2023, max compression
+gzip compressed data, was "codecarbon-2.2.4.tar", last modified: Wed Jun 21 08:40:51 2023, max compression
```

## Comparing `codecarbon-2.2.3.tar` & `codecarbon-2.2.4.tar`

### file list

```diff
@@ -1,119 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.112112 codecarbon-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-05 05:25:49.000000 codecarbon-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-05 05:26:02.112112 codecarbon-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-05 05:25:49.000000 codecarbon-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.100112 codecarbon-2.2.3/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/codecarbon/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/rapl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.100112 codecarbon-2.2.3/codecarbon/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/data/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/cloud/impact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/data/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    49423 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/hardware/cpu_power.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/data/private_infra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/data/private_infra/2016/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)    38065 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/emissions_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/geography.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.112112 codecarbon-2.2.3/codecarbon/viz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.112112 codecarbon-2.2.3/codecarbon/viz/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/carbonboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 05:26:02.112112 codecarbon-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-05 05:25:49.000000 codecarbon-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.112112 codecarbon-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_core_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_emissions_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_emissions_tracker_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_emissions_tracker_flush.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_geography.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_logging_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_ram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.903775 codecarbon-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 08:40:35.000000 codecarbon-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-21 08:40:51.903775 codecarbon-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-21 08:40:35.000000 codecarbon-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.879774 codecarbon-2.2.4/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.883774 codecarbon-2.2.4/carbonserver/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.883774 codecarbon-2.2.4/carbonserver/carbonserver/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.883774 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.887774 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.887774 codecarbon-2.2.4/carbonserver/carbonserver/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.887774 codecarbon-2.2.4/codecarbon/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/rapl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.879774 codecarbon-2.2.4/codecarbon/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/data/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/cloud/impact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/data/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    49423 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/hardware/cpu_power.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/data/private_infra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/data/private_infra/2016/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39720 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/emissions_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.895774 codecarbon-2.2.4/codecarbon/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.895774 codecarbon-2.2.4/codecarbon/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/prometheus/metric_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.895774 codecarbon-2.2.4/codecarbon/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.899775 codecarbon-2.2.4/codecarbon/viz/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/carbonboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.887774 codecarbon-2.2.4/codecarbon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:40:51.903775 codecarbon-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-21 08:40:36.000000 codecarbon-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.903775 codecarbon-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_core_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_emissions_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_emissions_tracker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_emissions_tracker_flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_logging_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/testutils.py
```

### Comparing `codecarbon-2.2.3/LICENSE` & `codecarbon-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/PKG-INFO` & `codecarbon-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.3
+Version: 2.2.4
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.3/README.md` & `codecarbon-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/dependencies.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/domain/experiments.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/domain/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/errors.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/errors.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/authenticate.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/emissions.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/experiments.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/organizations.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/organizations.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/projects.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/projects.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/runs.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/runs.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/teams.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/teams.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/users.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/api/schemas.py` & `codecarbon-2.2.4/carbonserver/carbonserver/api/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/carbonserver/database/database.py` & `codecarbon-2.2.4/carbonserver/carbonserver/database/database.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/container.py` & `codecarbon-2.2.4/carbonserver/container.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/main.py` & `codecarbon-2.2.4/carbonserver/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/carbonserver/setup.py` & `codecarbon-2.2.4/carbonserver/setup.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/cli/cli_utils.py` & `codecarbon-2.2.4/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/cli/main.py` & `codecarbon-2.2.4/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/api_client.py` & `codecarbon-2.2.4/codecarbon/core/api_client.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/cloud.py` & `codecarbon-2.2.4/codecarbon/core/cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/co2_signal.py` & `codecarbon-2.2.4/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/config.py` & `codecarbon-2.2.4/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/cpu.py` & `codecarbon-2.2.4/codecarbon/core/cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/emissions.py` & `codecarbon-2.2.4/codecarbon/core/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/gpu.py` & `codecarbon-2.2.4/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/rapl.py` & `codecarbon-2.2.4/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/schemas.py` & `codecarbon-2.2.4/codecarbon/core/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/units.py` & `codecarbon-2.2.4/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/core/util.py` & `codecarbon-2.2.4/codecarbon/core/util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/data/cloud/impact.csv` & `codecarbon-2.2.4/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.2.4/codecarbon/data/hardware/cpu_power.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.2.4/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.2.4/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.2.4/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/data/private_infra/global_energy_mix.json` & `codecarbon-2.2.4/codecarbon/data/private_infra/global_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/emissions_tracker.py` & `codecarbon-2.2.4/codecarbon/emissions_tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from codecarbon.output import (
     BaseOutput,
     CodeCarbonAPIOutput,
     EmissionsData,
     FileOutput,
     HTTPOutput,
     LoggerOutput,
+    PrometheusOutput,
 )
 
 # /!\ Warning: current implementation prevents the user from setting any value to None
 # from the script call
 # Imagine:
 #   1/ emissions_endpoint=localhost:8000 in ~/.codecarbon.config
 #   2/ Inside the script, the user cannot disable emissions_endpoint with
@@ -141,14 +142,16 @@
         api_key: Optional[str] = _sentinel,
         output_dir: Optional[str] = _sentinel,
         output_file: Optional[str] = _sentinel,
         save_to_file: Optional[bool] = _sentinel,
         save_to_api: Optional[bool] = _sentinel,
         save_to_logger: Optional[bool] = _sentinel,
         logging_logger: Optional[LoggerOutput] = _sentinel,
+        save_to_prometheus: Optional[bool] = _sentinel,
+        prometheus_url: Optional[str] = _sentinel,
         gpu_ids: Optional[List] = _sentinel,
         emissions_endpoint: Optional[str] = _sentinel,
         experiment_id: Optional[str] = _sentinel,
         co2_signal_api_token: Optional[str] = _sentinel,
         tracking_mode: Optional[str] = _sentinel,
         log_level: Optional[Union[int, str]] = _sentinel,
         on_csv_write: Optional[str] = _sentinel,
@@ -175,14 +178,17 @@
                              file, defaults to True.
         :param save_to_api: Indicates if the emission artifacts should be sent to the
                             CodeCarbon API, defaults to False.
         :param save_to_logger: Indicates if the emission artifacts should be written
                             to a dedicated logger, defaults to False.
         :param logging_logger: LoggerOutput object encapsulating a logging.logger
                             or a Google Cloud logger.
+        :param save_to_prometheus: Indicates if the emission artifacts should be
+                            pushed to prometheus, defaults to False.
+        :param prometheus_url: url of the prometheus server, defaults to `localhost:9091`.
         :param gpu_ids: User-specified known gpu ids to track, defaults to None.
         :param emissions_endpoint: Optional URL of http endpoint for sending emissions
                                    data.
         :param experiment_id: Id of the experiment.
         :param co2_signal_api_token: API token for co2signal.com (requires sign-up for
                                      free beta)
         :param tracking_mode: One of "process" or "machine" in order to measure the
@@ -215,19 +221,24 @@
         self._set_from_conf(output_dir, "output_dir", ".")
         self._set_from_conf(output_file, "output_file", "emissions.csv")
         self._set_from_conf(project_name, "project_name", "codecarbon")
         self._set_from_conf(save_to_api, "save_to_api", False, bool)
         self._set_from_conf(save_to_file, "save_to_file", True, bool)
         self._set_from_conf(save_to_logger, "save_to_logger", False, bool)
         self._set_from_conf(logging_logger, "logging_logger")
+        self._set_from_conf(save_to_prometheus, "save_to_prometheus", False, bool)
+        self._set_from_conf(prometheus_url, "prometheus_url", "localhost:9091")
         self._set_from_conf(tracking_mode, "tracking_mode", "machine")
         self._set_from_conf(on_csv_write, "on_csv_write", "append")
         self._set_from_conf(logger_preamble, "logger_preamble", "")
         self._set_from_conf(default_cpu_power, "default_cpu_power")
         self._set_from_conf(pue, "pue", 1.0, float)
+        self._set_from_conf(
+            experiment_id, "experiment_id", "5b0fa12a-3dd7-45bb-9766-cc326314d9f1"
+        )
 
         assert self._tracking_mode in ["machine", "process"]
         set_logger_level(self._log_level)
         set_logger_format(self._logger_preamble)
 
         self._start_time: Optional[float] = None
         self._last_measured_time: float = time.time()
@@ -235,14 +246,15 @@
         self._total_cpu_energy: Energy = Energy.from_energy(kWh=0)
         self._total_gpu_energy: Energy = Energy.from_energy(kWh=0)
         self._total_ram_energy: Energy = Energy.from_energy(kWh=0)
         self._cpu_power: Power = Power.from_watts(watts=0)
         self._gpu_power: Power = Power.from_watts(watts=0)
         self._ram_power: Power = Power.from_watts(watts=0)
         self._cc_api__out = None
+        self._cc_prometheus_out = None
         self._measure_occurrence: int = 0
         self._cloud = None
         self._previous_emissions = None
         self._conf["os"] = platform.platform()
         self._conf["python_version"] = platform.python_version()
         self._conf["cpu_count"] = count_cpus()
         self._geo = None
@@ -339,46 +351,53 @@
         else:
             self._conf["region"] = cloud.region
             self._conf["provider"] = cloud.provider
 
         self._emissions: Emissions = Emissions(
             self._data_source, self._co2_signal_api_token
         )
+        self._init_output_methods(api_key)
+
+    def _init_output_methods(self, api_key):
+        """
+        Prepare the different output methods
+        """
         self.persistence_objs: List[BaseOutput] = list()
 
         if self._save_to_file:
             self.persistence_objs.append(
                 FileOutput(
                     os.path.join(self._output_dir, self._output_file),
                     self._on_csv_write,
                 )
             )
 
         if self._save_to_logger:
             self.persistence_objs.append(self._logging_logger)
 
         if self._emissions_endpoint:
-            self.persistence_objs.append(HTTPOutput(emissions_endpoint))
+            self.persistence_objs.append(HTTPOutput(self._emissions_endpoint))
 
         if self._save_to_api:
-            experiment_id = self._set_from_conf(
-                experiment_id, "experiment_id", "5b0fa12a-3dd7-45bb-9766-cc326314d9f1"
-            )
             self._cc_api__out = CodeCarbonAPIOutput(
                 endpoint_url=self._api_endpoint,
-                experiment_id=experiment_id,
+                experiment_id=self._experiment_id,
                 api_key=api_key,
                 conf=self._conf,
             )
             self.run_id = self._cc_api__out.run_id
             self.persistence_objs.append(self._cc_api__out)
 
         else:
             self.run_id = uuid.uuid4()
 
+        if self._save_to_prometheus:
+            self._cc_prometheus_out = PrometheusOutput(self._prometheus_url)
+            self.persistence_objs.append(self._cc_prometheus_out)
+
     @suppress(Exception)
     def start(self) -> None:
         """
         Starts tracking the experiment.
         Currently, Nvidia GPUs are supported.
         :return: None
         """
@@ -591,22 +610,27 @@
                 + f"W during {last_duration:,.2f} s [measurement time: {h_time:,.4f}]"
             )
         logger.info(
             f"{self._total_energy.kWh:.6f} kWh of electricity used since the beginning."
         )
         self._last_measured_time = time.time()
         self._measure_occurrence += 1
-        if self._cc_api__out is not None and self._api_call_interval != -1:
+        if (
+            self._cc_api__out is not None or self._cc_prometheus_out is not None
+        ) and self._api_call_interval != -1:
             if self._measure_occurrence >= self._api_call_interval:
                 emissions = self._prepare_emissions_data(delta=True)
                 logger.info(
                     f"{emissions.emissions_rate * 1000:.6f} g.CO2eq/s mean an estimation of "
                     + f"{emissions.emissions_rate*3600*24*365:,} kg.CO2eq/year"
                 )
-                self._cc_api__out.out(emissions)
+                if self._cc_api__out:
+                    self._cc_api__out.out(emissions)
+                if self._cc_prometheus_out:
+                    self._cc_prometheus_out.out(emissions)
                 self._measure_occurrence = 0
         logger.debug(f"last_duration={last_duration}\n------------------------")
 
     def __enter__(self):
         self.start()
         return self
 
@@ -742,14 +766,16 @@
     api_endpoint: Optional[str] = _sentinel,
     api_key: Optional[str] = _sentinel,
     output_dir: Optional[str] = _sentinel,
     output_file: Optional[str] = _sentinel,
     save_to_file: Optional[bool] = _sentinel,
     save_to_api: Optional[bool] = _sentinel,
     save_to_logger: Optional[bool] = _sentinel,
+    save_to_prometheus: Optional[bool] = _sentinel,
+    prometheus_url: Optional[str] = _sentinel,
     logging_logger: Optional[LoggerOutput] = _sentinel,
     offline: Optional[bool] = _sentinel,
     emissions_endpoint: Optional[str] = _sentinel,
     experiment_id: Optional[str] = _sentinel,
     country_iso_code: Optional[str] = _sentinel,
     region: Optional[str] = _sentinel,
     cloud_provider: Optional[str] = _sentinel,
@@ -773,14 +799,17 @@
     :param output_file: Name of output CSV file, defaults to `emissions.csv`
     :param save_to_file: Indicates if the emission artifacts should be logged to a file,
                          defaults to True.
     :param save_to_api: Indicates if the emission artifacts should be send to the
                         CodeCarbon API, defaults to False.
     :param save_to_logger: Indicates if the emission artifacts should be written
                         to a dedicated logger, defaults to False.
+    :param save_to_prometheus: Indicates if the emission artifacts should be
+                            pushed to prometheus, defaults to False.
+    :param prometheus_url: url of the prometheus server, defaults to `localhost:9091`.
     :param logging_logger: LoggerOutput object encapsulating a logging.logger
                         or a Google Cloud logger.
     :param offline: Indicates if the tracker should be run in offline mode.
     :param country_iso_code: 3 letter ISO Code of the country where the experiment is
                              being run, required if `offline=True`
     :param region: The provice or region (e.g. California in the US).
                    Currently, this only affects calculations for the United States.
@@ -815,14 +844,16 @@
                 tracker = OfflineEmissionsTracker(
                     project_name=project_name,
                     measure_power_secs=measure_power_secs,
                     output_dir=output_dir,
                     output_file=output_file,
                     save_to_file=save_to_file,
                     save_to_logger=save_to_logger,
+                    save_to_prometheus=save_to_prometheus,
+                    prometheus_url=prometheus_url,
                     logging_logger=logging_logger,
                     country_iso_code=country_iso_code,
                     region=region,
                     cloud_provider=cloud_provider,
                     cloud_region=cloud_region,
                     gpu_ids=gpu_ids,
                     log_level=log_level,
@@ -834,14 +865,16 @@
                 tracker = EmissionsTracker(
                     project_name=project_name,
                     measure_power_secs=measure_power_secs,
                     output_dir=output_dir,
                     output_file=output_file,
                     save_to_file=save_to_file,
                     save_to_logger=save_to_logger,
+                    save_to_prometheus=save_to_prometheus,
+                    prometheus_url=prometheus_url,
                     logging_logger=logging_logger,
                     gpu_ids=gpu_ids,
                     log_level=log_level,
                     emissions_endpoint=emissions_endpoint,
                     experiment_id=experiment_id,
                     api_call_interval=api_call_interval,
                     api_key=api_key,
```

### Comparing `codecarbon-2.2.3/codecarbon/external/geography.py` & `codecarbon-2.2.4/codecarbon/external/geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/external/hardware.py` & `codecarbon-2.2.4/codecarbon/external/hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/external/logger.py` & `codecarbon-2.2.4/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/external/scheduler.py` & `codecarbon-2.2.4/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/input.py` & `codecarbon-2.2.4/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/output.py` & `codecarbon-2.2.4/codecarbon/output.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import pandas as pd
 import requests
 
 # from core.schema import EmissionCreate, Emission
 from codecarbon.core.api_client import ApiClient
 from codecarbon.core.util import backup
 from codecarbon.external.logger import logger
+from codecarbon.prometheus.prometheus import Prometheus
 
 
 @dataclass
 class EmissionsData:
     """
     Output object containg run data
     """
@@ -189,14 +190,29 @@
     def out(self, data: EmissionsData):
         try:
             self.api.add_emission(dataclasses.asdict(data))
         except Exception as e:
             logger.error(e, exc_info=True)
 
 
+class PrometheusOutput(BaseOutput):
+    """
+    Send emissions data to prometheus pushgateway
+    """
+
+    def __init__(self, prometheus_url: str):
+        self.prometheus = Prometheus(prometheus_url)
+
+    def out(self, data: EmissionsData):
+        try:
+            self.prometheus.add_emission(dataclasses.asdict(data))
+        except Exception as e:
+            logger.error(e, exc_info=True)
+
+
 class LoggerOutput(BaseOutput):
     """
     Send emissions data to a logger
     """
 
     def __init__(self, logger, severity=logging.INFO):
         self.logger = logger
```

### Comparing `codecarbon-2.2.3/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.2.4/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.2.4/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.2.4/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/viz/carbonboard.py` & `codecarbon-2.2.4/codecarbon/viz/carbonboard.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.2.4/codecarbon/viz/carbonboard_on_api.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/viz/components.py` & `codecarbon-2.2.4/codecarbon/viz/components.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon/viz/data.py` & `codecarbon-2.2.4/codecarbon/viz/data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/codecarbon.egg-info/PKG-INFO` & `codecarbon-2.2.4/codecarbon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.3
+Version: 2.2.4
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.3/codecarbon.egg-info/SOURCES.txt` & `codecarbon-2.2.4/codecarbon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 codecarbon/data/private_infra/2016/canada_energy_mix.json
 codecarbon/data/private_infra/2016/usa_emissions.json
 codecarbon/external/__init__.py
 codecarbon/external/geography.py
 codecarbon/external/hardware.py
 codecarbon/external/logger.py
 codecarbon/external/scheduler.py
+codecarbon/prometheus/__init__.py
+codecarbon/prometheus/metric_definitions.py
+codecarbon/prometheus/prometheus.py
 codecarbon/viz/__init__.py
 codecarbon/viz/carbonboard.py
 codecarbon/viz/carbonboard_on_api.py
 codecarbon/viz/components.py
 codecarbon/viz/data.py
 codecarbon/viz/assets/__init__.py
 codecarbon/viz/assets/car_icon.png
```

### Comparing `codecarbon-2.2.3/setup.py` & `codecarbon-2.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 
 TEST_DEPENDENCIES = ["mock", "pytest", "responses", "tox", "numpy", "requests-mock"]
 
 
 setuptools.setup(
     name="codecarbon",
-    version="2.2.3",
+    version="2.2.4",
     author="Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=("LICENSE",),
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
     ),
```

### Comparing `codecarbon-2.2.3/tests/test_api_call.py` & `codecarbon-2.2.4/tests/test_api_call.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_cloud.py` & `codecarbon-2.2.4/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_co2_signal.py` & `codecarbon-2.2.4/tests/test_co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_config.py` & `codecarbon-2.2.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_core_util.py` & `codecarbon-2.2.4/tests/test_core_util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_cpu.py` & `codecarbon-2.2.4/tests/test_cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_emissions.py` & `codecarbon-2.2.4/tests/test_emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_emissions_tracker.py` & `codecarbon-2.2.4/tests/test_emissions_tracker.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_emissions_tracker_constant.py` & `codecarbon-2.2.4/tests/test_emissions_tracker_constant.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_emissions_tracker_flush.py` & `codecarbon-2.2.4/tests/test_emissions_tracker_flush.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_energy.py` & `codecarbon-2.2.4/tests/test_energy.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_geography.py` & `codecarbon-2.2.4/tests/test_geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_gpu.py` & `codecarbon-2.2.4/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_hardware.py` & `codecarbon-2.2.4/tests/test_hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_logging_output.py` & `codecarbon-2.2.4/tests/test_logging_output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/test_ram.py` & `codecarbon-2.2.4/tests/test_ram.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/testdata.py` & `codecarbon-2.2.4/tests/testdata.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.3/tests/testutils.py` & `codecarbon-2.2.4/tests/testutils.py`

 * *Files identical despite different names*

