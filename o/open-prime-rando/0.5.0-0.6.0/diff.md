# Comparing `tmp/open-prime-rando-0.5.0.tar.gz` & `tmp/open-prime-rando-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-prime-rando-0.5.0.tar", last modified: Mon Jun 19 22:52:45 2023, max compression
+gzip compressed data, was "open-prime-rando-0.6.0.tar", last modified: Wed Jun 21 08:42:30 2023, max compression
```

## Comparing `open-prime-rando-0.5.0.tar` & `open-prime-rando-0.6.0.tar`

### file list

```diff
@@ -1,84 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/open_prime_rando/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/open_prime_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/dynamic_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/open_prime_rando/echoes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/agon_wastes.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/great_temple.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m02_spires.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m04_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/temple_grounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/torvus_bog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/auto_enabled_elevator_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.279379 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/dock_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/map_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/area_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/echo_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/rubiks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/specific_area_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/p1r_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/open_prime_rando/prime_remastered/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/prime_remastered/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/unique_area_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/open_prime_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/tests/test_echoes_custom_Assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/tools/asset_id_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.519227 open-prime-rando-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.495225 open-prime-rando-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.495225 open-prime-rando-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 08:42:30.519227 open-prime-rando-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.499225 open-prime-rando-0.6.0/open_prime_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.503226 open-prime-rando-0.6.0/open_prime_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/dynamic_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.507226 open-prime-rando-0.6.0/open_prime_rando/echoes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.511226 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/agon_wastes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/great_temple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/m02_spires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/m04_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/temple_grounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/torvus_bog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.491225 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.511226 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.515226 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/rubiks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.515226 open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/dock_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/map_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.515226 open-prime-rando-0.6.0/open_prime_rando/echoes/elevators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/elevators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/elevators/elevator_rando.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.515226 open-prime-rando-0.6.0/open_prime_rando/echoes/inverted/
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/inverted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/inverted/area_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.519227 open-prime-rando-0.6.0/open_prime_rando/echoes/small_randomizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/small_randomizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/small_randomizations/echo_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/small_randomizations/rubiks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/specific_area_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes/vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/echoes_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/p1r_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.519227 open-prime-rando-0.6.0/open_prime_rando/prime_remastered/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/prime_remastered/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/unique_area_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/open_prime_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 08:42:30.000000 open-prime-rando-0.6.0/open_prime_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.503226 open-prime-rando-0.6.0/open_prime_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 08:42:30.000000 open-prime-rando-0.6.0/open_prime_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-21 08:42:30.000000 open-prime-rando-0.6.0/open_prime_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:42:30.000000 open-prime-rando-0.6.0/open_prime_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 08:42:30.000000 open-prime-rando-0.6.0/open_prime_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:42:30.000000 open-prime-rando-0.6.0/open_prime_rando.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 08:42:30.000000 open-prime-rando-0.6.0/open_prime_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 08:42:30.000000 open-prime-rando-0.6.0/open_prime_rando.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-21 08:42:30.519227 open-prime-rando-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.519227 open-prime-rando-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/tests/test_echoes_custom_Assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:42:30.519227 open-prime-rando-0.6.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-21 08:42:07.000000 open-prime-rando-0.6.0/tools/asset_id_files.py
```

### Comparing `open-prime-rando-0.5.0/.github/dependabot.yml` & `open-prime-rando-0.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/.github/workflows/python.yml` & `open-prime-rando-0.6.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/.gitignore` & `open-prime-rando-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/LICENSE` & `open-prime-rando-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/PKG-INFO` & `open-prime-rando-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.5.0
+Version: 0.6.0
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Home-page: https://github.com/randovania/open-prime-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/cli.py` & `open-prime-rando-0.6.0/open_prime_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/dynamic_schema.py` & `open-prime-rando-0.6.0/open_prime_rando/dynamic_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     world_props = schema["properties"]["worlds"]["properties"] = {}
     for world, mlvl_id in open_prime_rando.echoes.asset_ids.world.NAME_TO_ID_MLVL.items():
         world_def = copy.deepcopy(schema["$defs"]["world"])
         world_props[world] = world_def
 
         mlvl = editor.get_mlvl(mlvl_id)
         area_props = {}
-        # FIXME: setting it to True for now to fix elevator rooms breaking when renamed
-        world_def["properties"]["areas"] = {"type": "object", "additionalProperties": True, "properties": area_props}
+        world_def["properties"]["areas"] = {"type": "object", "additionalProperties": False, "properties": area_props}
 
         world_details = open_prime_rando.echoes.asset_ids.world.load_dedicated_file(world)
 
         for area in mlvl.areas:
             area_name = get_name_for_area(area)
             area_def = copy.deepcopy(schema["$defs"]["area"])
             area_props[area_name] = area_def
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/agon_wastes.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/agon_wastes.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/great_temple.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/great_temple.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/temple_grounds.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/temple_grounds.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/torvus_bog.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/torvus_bog.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/world.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/asset_ids/world.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/auto_enabled_elevator_patches.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 import open_prime_rando.echoes.asset_ids.agon_wastes as agon_wastes
 import open_prime_rando.echoes.asset_ids.great_temple as great_temple
 import open_prime_rando.echoes.asset_ids.sanctuary_fortress as sanctuary_fortress
 import open_prime_rando.echoes.asset_ids.temple_grounds as temple_grounds
 import open_prime_rando.echoes.asset_ids.torvus_bog as torvus_bog
+import open_prime_rando.echoes.asset_ids.world as world
 from open_prime_rando.patcher_editor import PatcherEditor
 
 from retro_data_structures.formats.script_object import ScriptInstanceHelper
 from retro_data_structures.game_check import Game
 from retro_data_structures.properties.echoes.objects.Timer import Timer
+from retro_data_structures.properties.echoes.archetypes.EditorProperties import EditorProperties
+from retro_data_structures.enums.echoes import State, Message
+
 
 ELEVATOR_MEMORY_RELAY_PER_MREA = {
-    # Great Temple elevators
-    great_temple.TEMPLE_TRANSPORT_A_MREA: 0x00000107,
-    great_temple.TEMPLE_TRANSPORT_B_MREA: 0x0008002f,
-    great_temple.TEMPLE_TRANSPORT_C_MREA: 0x00060046,
-    # Temple Grounds elevators
-    temple_grounds.TRANSPORT_TO_AGON_WASTES_MREA: 0x00180040,
-    temple_grounds.TRANSPORT_TO_SANCTUARY_FORTRESS_MREA: 0x00330058,
-    temple_grounds.TRANSPORT_TO_TORVUS_BOG_MREA: 0x001e0061,
-    # Agon Wastes elevators
-    agon_wastes.TRANSPORT_TO_SANCTUARY_FORTRESS_MREA: 0x002d0064,
-    agon_wastes.TRANSPORT_TO_TEMPLE_GROUNDS_MREA: 0x0000003f,
-    agon_wastes.TRANSPORT_TO_TORVUS_BOG_MREA: 0x0013004d,
-    # Torvus Bog elevators
-    torvus_bog.TRANSPORT_TO_AGON_WASTES_MREA: 0x00210038,
-    torvus_bog.TRANSPORT_TO_SANCTUARY_FORTRESS_MREA: 0x0045004b,
-    torvus_bog.TRANSPORT_TO_TEMPLE_GROUNDS_MREA: 0x0000002e,
-    # Sanctuary Fortress elevators
-    sanctuary_fortress.TRANSPORT_TO_AGON_WASTES_MREA: 0x00130088,
-    sanctuary_fortress.TRANSPORT_TO_TEMPLE_GROUNDS_MREA: 0x00000035,
-    sanctuary_fortress.TRANSPORT_TO_TORVUS_BOG_MREA: 0x00190036,
+    world.GREAT_TEMPLE_MLVL: {
+        great_temple.TEMPLE_TRANSPORT_A_MREA: 0x00000107,
+        great_temple.TEMPLE_TRANSPORT_B_MREA: 0x0008002f,
+        great_temple.TEMPLE_TRANSPORT_C_MREA: 0x00060046,
+    },
+
+    world.TEMPLE_GROUNDS_MLVL: {
+        temple_grounds.TRANSPORT_TO_AGON_WASTES_MREA: 0x00180040,
+        temple_grounds.TRANSPORT_TO_SANCTUARY_FORTRESS_MREA: 0x00330058,
+        temple_grounds.TRANSPORT_TO_TORVUS_BOG_MREA: 0x001e0061,
+    },
+
+    world.AGON_WASTES_MLVL: {
+        agon_wastes.TRANSPORT_TO_SANCTUARY_FORTRESS_MREA: 0x002d0064,
+        agon_wastes.TRANSPORT_TO_TEMPLE_GROUNDS_MREA: 0x0000003f,
+        agon_wastes.TRANSPORT_TO_TORVUS_BOG_MREA: 0x0013004d,
+    },
+
+    world.TORVUS_BOG_MLVL: {
+        torvus_bog.TRANSPORT_TO_AGON_WASTES_MREA: 0x00210038,
+        torvus_bog.TRANSPORT_TO_SANCTUARY_FORTRESS_MREA: 0x0045004b,
+        torvus_bog.TRANSPORT_TO_TEMPLE_GROUNDS_MREA: 0x0000002e,
+    },
+
+    world.SANCTUARY_FORTRESS_MLVL: {
+        sanctuary_fortress.TRANSPORT_TO_AGON_WASTES_MREA: 0x00130088,
+        sanctuary_fortress.TRANSPORT_TO_TEMPLE_GROUNDS_MREA: 0x00000035,
+        sanctuary_fortress.TRANSPORT_TO_TORVUS_BOG_MREA: 0x00190036,
+    }
 }
 
 
 def apply_auto_enabled_elevators_patch(editor: PatcherEditor):
     """
     Patches that activates every elevator on room load
     """
-    for elevator_mrea, memory_relay_id in ELEVATOR_MEMORY_RELAY_PER_MREA.items():
-        area = editor.get_mrea(elevator_mrea)
-        layers = area.script_layers()
-        layer = [layer for layer in layers if layer.name() == "Default"][0]
-
-        """
-        Add timer that activates the memory relay of the elevator hologram
-        """
-        timer = ScriptInstanceHelper.new_instance(Game.ECHOES, "TIMR", layer)
-        properties = timer.get_properties_as(Timer)
-
-        properties.editor_properties.transform.position = [0.000000, 0.000000, 0.000000]
-        properties.editor_properties.transform.rotation = [0.000000, 0.000000, 0.000000]
-        properties.editor_properties.transform.scale = [1.000000, 1.000000, 1.000000]
-        properties.editor_properties.name = "Timer - Auto enable elevator"
-        properties.editor_properties.active = 0
-        properties.editor_properties.unknown = 3
-        properties.time = 0.001
-        properties.random_adjust = 0.0
-        properties.auto_reset = False
-        properties.auto_start = True
-
-        timer.add_connection("ZERO", "ACTV", memory_relay_id)
-
+    for mlvl_id, areas in ELEVATOR_MEMORY_RELAY_PER_MREA.items():
+        for mrea_id, memory_relay_id in areas.items():
+            area = editor.get_area_helper(mlvl_id, mrea_id)
+            timer = area.get_layer("Default").add_instance_with(Timer(
+                editor_properties=EditorProperties(
+                    name="Timer - Auto enable elevator",
+                    active=False
+                ),
+                time=0.001,
+                auto_start=True
+            ))
+            relay = area.get_instance(memory_relay_id)
+            timer.add_connection(State.Zero, Message.Activate, relay)
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR` & `open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR` & `open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR` & `open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR` & `open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR` & `open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR` & `open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR` & `open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/custom_assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/__init__.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/dock_type.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/dock_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 import dataclasses
 import functools
 import logging
+from typing import NamedTuple, Type
 from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
 from open_prime_rando.patcher_editor import PatcherEditor
 from open_prime_rando.echoes.asset_ids import *
+from open_prime_rando.echoes.vulnerabilities import resist_all_vuln
 
 from retro_data_structures.base_resource import AssetId
 from retro_data_structures.asset_manager import NameOrAssetId
+from retro_data_structures.properties.base_property import BaseObjectType
 from retro_data_structures.properties.echoes.archetypes.DamageVulnerability import DamageVulnerability
 from retro_data_structures.properties.echoes.archetypes.WeaponVulnerability import WeaponVulnerability
 from retro_data_structures.properties.echoes.core.Color import Color
 from retro_data_structures.properties.echoes.core.Vector import Vector
 from retro_data_structures.properties.echoes.archetypes.EditorProperties import EditorProperties
 from retro_data_structures.properties.echoes.archetypes.ScannableParameters import ScannableParameters
 from retro_data_structures.properties.echoes.archetypes.SurroundPan import SurroundPan
 from retro_data_structures.properties.echoes.archetypes.ActorParameters import ActorParameters
+from retro_data_structures.properties.echoes.archetypes.HealthInfo import HealthInfo
+from retro_data_structures.properties.echoes.archetypes.VisorParameters import VisorParameters
+from retro_data_structures.properties.echoes.archetypes.Transform import Transform
 from retro_data_structures.properties.echoes.objects.Dock import Dock
 from retro_data_structures.properties.echoes.objects.Door import Door
 from retro_data_structures.properties.echoes.objects.Actor import Actor
 from retro_data_structures.properties.echoes.objects.MemoryRelay import MemoryRelay
 from retro_data_structures.properties.echoes.objects.ScannableObjectInfo import ScannableObjectInfo
 from retro_data_structures.properties.echoes.objects.Sound import Sound
 from retro_data_structures.properties.echoes.objects.StreamedAudio import StreamedAudio
 from retro_data_structures.properties.echoes.objects.MemoryRelay import MemoryRelay
 from retro_data_structures.properties.echoes.objects.Effect import Effect
+from retro_data_structures.properties.echoes.objects.DamageableTrigger import DamageableTrigger
+from retro_data_structures.properties.echoes.objects.DamageableTriggerOrientated import DamageableTriggerOrientated
+from retro_data_structures.properties.echoes.objects.Timer import Timer
+from retro_data_structures.properties.echoes.objects.CameraShaker import CameraShaker
+from retro_data_structures.properties.echoes.objects.Counter import Counter
+from retro_data_structures.properties.echoes.objects.Relay import Relay
 from retro_data_structures.properties.echoes.core.Spline import Spline
 from retro_data_structures.formats.mapa import Mapa
 from retro_data_structures.formats.mlvl import AreaWrapper
 from retro_data_structures.formats.scan import Scan
 from retro_data_structures.formats.strg import Strg
-from retro_data_structures.formats.script_object import ScriptInstanceHelper, InstanceId
-from retro_data_structures.enums.echoes import State, Message
+from retro_data_structures.formats.script_object import ScriptInstanceHelper
+from retro_data_structures.enums.echoes import State, Message, VisorFlags
 
 
 @dataclasses.dataclass(kw_only=True)
 class DoorType:
     name: str
 
     vulnerability: DamageVulnerability
@@ -53,22 +65,22 @@
         return editor.find_paks(world_file.NAME_TO_ID_MREA[area_name])
 
     def get_files(self, editor: PatcherEditor, world_name: str, area_name: str) -> tuple[AreaWrapper, Mapa]:
         world_file = world.load_dedicated_file(world_name)
         mrea = editor.get_area_helper(world.NAME_TO_ID_MLVL[world_name], world_file.NAME_TO_ID_MREA[area_name])
         mapa = editor.get_file(world_file.NAME_TO_ID_MAPA[area_name], type_hint=Mapa)
         return mrea, mapa
-    
+
     def get_dock_index(self, world_name: str, area_name: str, dock_name: str) -> int:
         world_file = world.load_dedicated_file(world_name)
         return world_file.DOCK_NAMES[area_name][dock_name]
-    
+
     def get_mrea(self, editor: PatcherEditor, world_name: str, area_name: str) -> AreaWrapper:
         return self.get_files(editor, world_name, area_name)[0]
-    
+
     def get_door_from_dock_index(self, mrea: AreaWrapper, dock_index: int) -> ScriptInstanceHelper:
         dock = next(
             inst for inst in mrea.mrea.all_instances
             if (
                 inst.type == Dock and
                 inst.get_properties_as(Dock).dock_number == dock_index
             )
@@ -82,148 +94,161 @@
         raise KeyError(f"no door found with a connection to {dock} in {mrea.name}")
 
     def patch_map_icon(self, mapa: Mapa, door: ScriptInstanceHelper):
         for obj in mapa.raw.mappable_objects:
             if door.id_matches(obj.editor_id):
                 obj.type = self.map_icon.value
                 return
-    
+
     @staticmethod
     def get_scan_templates(editor: PatcherEditor) -> tuple[Scan, Strg]:
         # Uncategorized/There is a Blast Shield on the door blocking acces_0.SCAN
         scan = editor.get_parsed_asset(0x36DE1342, type_hint=Scan)
         # Strings/Uncategorized/There is a Blast Shield on the door blocking acces_0_0.STRG
         strg = editor.get_parsed_asset(0x49DF4448, type_hint=Strg)
         return scan, strg
 
     def get_patched_scan(self, editor: PatcherEditor, world_name: str, area_name: str) -> AssetId:
         paks = self.get_paks(editor, world_name, area_name)
         if self.patched_scan is None or not editor.does_asset_exists(self.patched_scan):
             scan, strg = DoorType.get_scan_templates(editor)
             for i, text in enumerate(self.scan_text):
                 strg.set_string(i, text)
-            
+
             strg_id = editor.add_or_replace_custom_asset(f"custom_door_{self.name}.STRG", strg, paks)
 
-            scan_info = scan.scannable_object_info.get_properties_as(ScannableObjectInfo)
-            scan_info.string = strg_id
-            scan.scannable_object_info.set_properties(scan_info)
+            with scan.scannable_object_info.edit_properties(ScannableObjectInfo) as scan_info:
+                scan_info.string = strg_id
 
             scan_id = editor.add_or_replace_custom_asset(f"custom_door_{self.name}.SCAN", scan, paks)
             self.patched_scan = scan_id
-        
+
         for pak in paks:
             editor.ensure_present(pak, self.patched_scan)
         return self.patched_scan
 
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         mrea, mapa = self.get_files(editor, world_name, area_name)
         door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
         self.patch_map_icon(mapa, door)
 
         shell_model = editor._resolve_asset_id(self.shell_model)
 
-        door_props = door.get_properties_as(Door)
-        door_props.shell_model = shell_model
-        door_props.shell_color = self.shell_color
-        door.set_properties(door_props)
+        with door.edit_properties(Door) as door_props:
+            door_props.shell_model = shell_model
+            door_props.shell_color = self.shell_color
 
         for pak in self.get_paks(editor, world_name, area_name):
             editor.ensure_present(pak, shell_model)
 
 
 @dataclasses.dataclass(kw_only=True)
 class NormalDoorType(DoorType):
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         super().patch_door(editor, world_name, area_name, dock_name, low_memory)
         mrea = self.get_mrea(editor, world_name, area_name)
         door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
-        
-        door_props = door.get_properties_as(Door)
-        door_props.vulnerability = self.vulnerability
-
-        if self.scan_text is not None:
-            door_props.alt_scannable.scannable_info0 = self.get_patched_scan(editor, world_name, area_name)
-        
-        door.set_properties(door_props)
-    
+
+        with door.edit_properties(Door) as door_props:
+            door_props.vulnerability = self.vulnerability
+            if self.scan_text is not None:
+                door_props.alt_scannable.scannable_info0 = self.get_patched_scan(editor, world_name, area_name)
+
+
+class BlastShieldActors(NamedTuple):
+    door: ScriptInstanceHelper
+    sound: ScriptInstanceHelper
+    streamed: ScriptInstanceHelper
+    lock: ScriptInstanceHelper
+    relay: ScriptInstanceHelper
+    gibs: ScriptInstanceHelper | None
+
 
 @dataclasses.dataclass(kw_only=True)
 class BlastShieldDoorType(DoorType):
     shield_model: NameOrAssetId
     shield_collision_box: Vector = dataclasses.field(default_factory=lambda: Vector(0.35, 5.0, 4.0))
     shield_collision_offset: Vector = dataclasses.field(default_factory=lambda: Vector(-2/3, 0, 2.0))
-    
+
+    def find_attached_instance(self, area: AreaWrapper, source: ScriptInstanceHelper, state: State, message: Message, target_type: Type[BaseObjectType], target_name: str | None = None) -> ScriptInstanceHelper:
+        for connection in source.connections:
+            if connection.state == state and connection.message == message:
+                target = area.get_instance(connection.target)
+                if target.type == target_type and (target_name is None or target.name == target_name):
+                    return target
+        name = f"{target_type} named {target_name}" if target_name is not None else str(target_type)
+        raise TypeError(f"No {name} connected to {source}")
+
     def get_spline(self) -> Spline:
         return Spline(data=b'\x00\x00\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x02\x02A \x00\x00?\x80\x00\x00\x02\x02\x01\x00\x00\x00\x00?\x80\x00\x00')
 
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         """
         blast shield connections:
             DEAD -> lock cleared MemoryRelay, ACTV
             DEAD -> lock breaking SoundEffect, PLAY
             DEAD -> lock explosion gibs, ACTV
             DEAD -> jingle streamedaudio, PLAY
-        
+
         door connections:
             OPEN -> lock cleared MemoryRelay, ACTV
-        
+
         memory relay connections:
             ACTV -> door, RSET
             ACTV -> blast shield, DCTV
         """
         super().patch_door(editor, world_name, area_name, dock_name, low_memory)
         mrea = self.get_mrea(editor, world_name, area_name)
         door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
-        _door = door.get_properties_as(Door)
+        door_transform = door.get_properties_as(Door).editor_properties.transform
 
         default = mrea.get_layer("Default")
-        
+
         sound = default.add_instance_with(Sound(
             editor_properties=EditorProperties(
                 name="Metal Door Lock Breaking",
-                transform=_door.editor_properties.transform
+                transform=door_transform
             ),
             sound=948,
             max_audible_distance=150.0,
             surround_pan=SurroundPan(surround_pan=1.0)
         ))
 
         streamed = default.add_instance_with(StreamedAudio(
             editor_properties=EditorProperties(
                 name="StreamedAudio - Event Jingle",
-                transform=_door.editor_properties.transform
+                transform=door_transform
             ),
             song_file="/audio/evt_x_event_00.dsp",
             fade_in_time=0.01,
             volume=65,
             software_channel=1,
             unknown=False
         ))
 
         model = editor._resolve_asset_id(self.shield_model)
         lock = default.add_instance_with(Actor(
             editor_properties=EditorProperties(
                 name=f"{self.name} Blast Shield Lock",
-                transform=_door.editor_properties.transform
+                transform=door_transform
             ),
             collision_box=self.shield_collision_box,
             collision_offset=self.shield_collision_offset,
             vulnerability=self.vulnerability,
             model=model,
             actor_information=ActorParameters(
                 scannable=ScannableParameters(
                     scannable_info0=self.get_patched_scan(editor, world_name, area_name)
                 )
             )
         ))
 
         relay = default.add_memory_relay("Lock Cleared")
         with relay.edit_properties(MemoryRelay) as _relay:
-            _relay.editor_properties.transform = _door.editor_properties.transform
+            _relay.editor_properties.transform = door_transform
             _relay.editor_properties.active = False
 
         lock.add_connection(State.Dead, Message.Play, sound)
         lock.add_connection(State.Dead, Message.Play, streamed)
         lock.add_connection(State.Dead, Message.Activate, relay)
 
         relay.add_connection(State.Active, Message.Deactivate, lock)
@@ -232,76 +257,161 @@
         door.add_connection(State.Open, Message.Activate, relay)
 
         dependencies = [
             model,
             0x8B4CD966, # MetalDoorLockBreak AGSC
         ]
 
+        gibs = None
         if not low_memory:
             particle = 0xCDCBDF04
 
             gibs = default.add_instance_with(Effect(
                 editor_properties=EditorProperties(
-                    transform=_door.editor_properties.transform,
+                    transform=door_transform,
                     active=False
                 ),
                 particle_effect=particle,
                 restart_on_activate=True,
                 motion_control_spline=self.get_spline(),
             ))
 
             lock.add_connection(State.Dead, Message.Activate, gibs)
             dependencies.append(particle)
 
         for pak in self.get_paks(editor, world_name, area_name):
             for asset in dependencies:
                 editor.ensure_present(pak, asset)
 
-    
+        return BlastShieldActors(door, sound, streamed, lock, relay, gibs)
+
 
 @dataclasses.dataclass(kw_only=True)
 class VanillaBlastShieldDoorType(BlastShieldDoorType):
     def remove_blast_shield(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str):
         mrea = self.get_mrea(editor, world_name, area_name)
         door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
 
-        relay = None
-        for connection in door.connections:
-            if connection.state == State.Open and connection.message == Message.Activate:
-                target = mrea.get_instance(connection.target)
-                if target.type == MemoryRelay:
-                    relay = target
-                    break
-        
-        if relay is None:
-            raise TypeError(f"No MemoryRelay connected to {door} in {world_name}/{area_name}")
-        
-        lock = None
-        for connection in relay.connections:
-            if connection.state == State.Active and connection.message == Message.Deactivate:
-                target = mrea.get_instance(connection.target)
-                if target.type == Actor:
-                    lock = target
-                    break
-        
-        if lock is None:
-            raise TypeError(f"No lock Actor connected to {relay} in {world_name}/{area_name}")
-        
+        relay = self.find_attached_instance(mrea, door, State.Open, Message.Activate, MemoryRelay)
+        lock = self.find_attached_instance(mrea, relay, State.Active, Message.Deactivate, Actor)
+
         for connection in lock.connections:
             mrea.mrea.remove_instance(connection.target)
         mrea.mrea.remove_instance(lock)
 
 
 @dataclasses.dataclass(kw_only=True)
 class SeekerBlastShieldDoorType(VanillaBlastShieldDoorType):
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
-        raise NotImplementedError()
-    
+        actors = super().patch_door(editor, world_name, area_name, dock_name, low_memory)
+        mrea = self.get_mrea(editor, world_name, area_name)
+        default = mrea.get_layer("Default")
+
+        # immune instead of reflect so that it explodes on the lock
+        missile_immune = dataclasses.replace(resist_all_vuln, missile=WeaponVulnerability(damage_multiplier=0.0))
+        with actors.lock.edit_properties(Actor) as lock:
+            lock.vulnerability = missile_immune
+        with actors.door.edit_properties(Door) as door:
+            door.vulnerability = missile_immune
+
+        door_transform = actors.door.get_properties_as(Door).editor_properties.transform
+
+        def create_trigger(name: str, health: float, lock_on: bool = True) -> ScriptInstanceHelper:
+            pos = Vector(
+                door_transform.position.x,
+                door_transform.position.y,
+                door_transform.position.z + 1.8
+            )
+
+            return default.add_instance_with(DamageableTriggerOrientated(
+                editor_properties=EditorProperties(
+                    name=name,
+                    transform=Transform(
+                        position=pos,
+                        rotation=door_transform.rotation,
+                        scale=Vector(4.0, 4.0, 1.5)
+                    ),
+                ),
+                health=HealthInfo(health=health),
+                vulnerability=self.vulnerability,
+                enable_seeker_lock_on=lock_on,
+                visor=VisorParameters(
+                    visor_flags=VisorFlags.Combat | VisorFlags.Dark
+                )
+            ))
+
+        timer = default.add_instance_with(Timer(
+            editor_properties=EditorProperties(
+                name="Button Control",
+                transform=door_transform
+            ),
+            time=0.75
+        ))
+
+        timer_reset = default.add_instance_with(Timer(
+            editor_properties=EditorProperties(
+                name="Button Reset",
+                transform=door_transform
+            ),
+            time=0.01
+        ))
+
+        # create 5 triggers so that you can have 5 lock-ons
+        # 30.01 health because splash damage is inconsistent. missiles do 30 damage
+        # so this guarantees you need at least 2 missiles at once to break it
+        triggers = [create_trigger(f"Bridge Button {i}", 30.01) for i in range(5)]
+        main_trigger = triggers[0]
+        mini_trigger = create_trigger("Bridge Button Mini", 1.0, False)
+
+        # start a timer when the tiny trigger dies. stop it if the main trigger dies
+        mini_trigger.add_connection(State.Dead, Message.ResetAndStart, timer)
+        main_trigger.add_connection(State.Dead, Message.Stop, timer)
+        for trigger in triggers:
+            timer.add_connection(State.Zero, Message.Deactivate, trigger)
+
+        # if the timer counts all the way down, reset the triggers
+        timer.add_connection(State.Zero, Message.ResetAndStart, timer_reset)
+        timer_reset.add_connection(State.Zero, Message.Activate, mini_trigger)
+        for trigger in triggers:
+            timer_reset.add_connection(State.Zero, Message.Activate, trigger)
+
+        # move the lock's connections to the trigger, since it's the thing that dies now
+        for connection in actors.lock.connections:
+            actors.lock.remove_connection(connection)
+            main_trigger.add_connection(
+                connection.state,
+                connection.message,
+                default.get_instance(connection.target)
+            )
+
+        for trigger in triggers:
+            actors.relay.add_connection(State.Active, Message.Deactivate, trigger)
+
+
     def remove_blast_shield(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str):
-        raise NotImplementedError()
+        mrea = self.get_mrea(editor, world_name, area_name)
+        door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
+
+        default = mrea.get_layer("Default")
+
+        memory_relay = self.find_attached_instance(mrea, door, State.Open, Message.Activate, MemoryRelay)
+        trigger = self.find_attached_instance(mrea, memory_relay, State.Active, Message.Deactivate, DamageableTrigger)
+        shaker = self.find_attached_instance(mrea, trigger, State.Dead, Message.Action, CameraShaker)
+        counter = self.find_attached_instance(mrea, trigger, State.Dead, Message.Increment, Counter)
+        complete_relay = self.find_attached_instance(mrea, counter, State.MaxReached, Message.SetToZero, Relay)
+
+        default.remove_instance(shaker)
+        for connection in complete_relay.connections:
+            try:
+                default.remove_instance(connection.target)
+            except KeyError:
+                # I guess claris already removed it probably?
+                complete_relay.remove_connection(connection)
+        default.remove_instance(complete_relay)
+        default.remove_instance(counter)
 
 
 @dataclasses.dataclass(kw_only=True)
 class PlanetaryEnergyDoorType(DoorType):
     planetary_energy_item_id: int
 
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
@@ -334,8 +444,7 @@
 
 @dataclasses.dataclass(kw_only=True)
 class TranslatorDoorType(ScanVisorDoorType):
     translator_item_id: int
 
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         raise NotImplementedError()
-
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,25 @@
 import dataclasses
 
-from retro_data_structures.enums import echoes
-from retro_data_structures.properties.echoes.archetypes.DamageVulnerability import DamageVulnerability
-from retro_data_structures.properties.echoes.archetypes.WeaponVulnerability import WeaponVulnerability
 from retro_data_structures.properties.echoes.core.Color import Color
 from retro_data_structures.properties.echoes.core.Vector import Vector
-from retro_data_structures.crc import crc32
 
 from open_prime_rando.echoes.dock_lock_rando.dock_type import *
 from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
+from open_prime_rando.echoes.vulnerabilities import vulnerable, resist_all_vuln
 
-reflect = WeaponVulnerability(damage_multiplier=0, effect=echoes.Effect.Reflect)
-vulnerable = WeaponVulnerability(damage_multiplier=100, effect=echoes.Effect.Normal)
-immune = WeaponVulnerability(damage_multiplier=0, effect=echoes.Effect.Normal, ignore_radius=True)
-
-resist_all_vuln = DamageVulnerability(
-    power=reflect, dark=reflect, light=reflect, annihilator=reflect,
-    power_charge=reflect, entangler=reflect, light_blast=reflect, sonic_boom=reflect,
-    super_missle=reflect, black_hole=reflect, sunburst=reflect, imploder=reflect,
-
-    boost_ball=immune, cannon_ball=immune, screw_attack=immune, bomb=immune, power_bomb=immune,
-    missile=immune, phazon=reflect, ai=immune, poison_water=immune, dark_water=immune, lava=immune,
-    area_damage_hot=immune, area_damage_cold=immune, area_damage_dark=immune, area_damage_light=immune,
-    weapon_vulnerability=immune, normal_safe_zone=immune,
-)
 
 normal_door_model = 0x6B78FD92
 dark_door_model = 0xbbcf134d
 annihilator_door_model = 0xa50c7238
 
 blast_collision_box = Vector(0.35, 5.0, 4.0)
 blast_collision_offset = Vector(-2/3, 0, 2.0)
 
+
 DOCK_TYPES: dict[str, DoorType] = {
     "Normal": NormalDoorType(
         name="Normal",
         vulnerability=dataclasses.replace(
             resist_all_vuln,
             power=vulnerable, dark=vulnerable, light=vulnerable, annihilator=vulnerable,
             power_charge=vulnerable, entangler=vulnerable, light_blast=vulnerable, sonic_boom=vulnerable,
@@ -124,15 +108,15 @@
     ),
     "SeekerMissile": SeekerBlastShieldDoorType(
         name="SeekerMissile",
         vulnerability=dataclasses.replace(resist_all_vuln, missile=vulnerable),
         shell_color=Color(r=0.5, g=0, b=0.64, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to most weapons. Five simultaneous blasts from Seeker Missiles may damage it."
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. Five simultaneous Missile blasts may damage it."
         ),
         map_icon=DoorMapIcon.SeekerMissile,
         shield_model=0x56F4208B,
     ),
     "ScrewAttack": BlastShieldDoorType(
         name="ScrewAttack",
         vulnerability=dataclasses.replace(resist_all_vuln, screw_attack=vulnerable),
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/map_icons.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/dock_lock_rando/map_icons.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/__init__.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/inverted/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/area_pairs.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/inverted/area_pairs.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/schema.json` & `open-prime-rando-0.6.0/open_prime_rando/echoes/schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827314814814815%*

 * *Differences: {"'$defs'": "{'area': {'properties': {'low_memory_mode': {'$comment': 'Some areas are riding the "*

 * *            'memory/object limit. Certain patches will account for these limitations if this flag '*

 * *            "is set.'}, 'new_name': OrderedDict([('type', ['string', 'null']), ('default', None), "*

 * *            "('$comment', 'If set, rename the area to this value')]), 'elevators': "*

 * *            "OrderedDict([('type', 'array'), ('items', OrderedDict([('type', 'object'), "*

 * *            "('properties', OrderedDic […]*

```diff
@@ -9,27 +9,78 @@
                     "patternProperties": {
                         ".*": {
                             "$ref": "#/$defs/dock"
                         }
                     },
                     "type": "object"
                 },
+                "elevators": {
+                    "default": [],
+                    "items": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "instance_id": {
+                                "type": "integer"
+                            },
+                            "target_assets": {
+                                "$ref": "#/$defs/area_identifier"
+                            },
+                            "target_name": {
+                                "type": "string"
+                            },
+                            "target_strg": {
+                                "default": null,
+                                "type": [
+                                    "integer",
+                                    "null"
+                                ]
+                            }
+                        },
+                        "required": [
+                            "instance_id",
+                            "target_assets",
+                            "target_name"
+                        ],
+                        "type": "object"
+                    },
+                    "type": "array"
+                },
                 "layers": {
                     "$comment": "The list of layers is replaced in runtime with the existing layers of each specific area.",
                     "default": {},
                     "patternProperties": {
                         ".*": {
                             "type": "boolean"
                         }
                     },
                     "type": "object"
                 },
                 "low_memory_mode": {
+                    "$comment": "Some areas are riding the memory/object limit. Certain patches will account for these limitations if this flag is set.",
                     "default": false,
                     "type": "boolean"
+                },
+                "new_name": {
+                    "$comment": "If set, rename the area to this value",
+                    "default": null,
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                }
+            },
+            "type": "object"
+        },
+        "area_identifier": {
+            "properties": {
+                "area_asset_id": {
+                    "type": "integer"
+                },
+                "world_asset_id": {
+                    "type": "integer"
                 }
             },
             "type": "object"
         },
         "dock": {
             "additionalProperties": false,
             "default": {},
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/__init__.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/small_randomizations/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 import random
 from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MINIGYRO_CHAMBER_MREA
 from open_prime_rando.patcher_editor import PatcherEditor
 
 from retro_data_structures.formats.strg import Strg
+from retro_data_structures.enums.echoes import State, Message
 
 
 class GyroColor(Enum):
     AMBER = 0
     COBALT = 1
     CRIMSON = 2
     EMERALD = 3
@@ -18,41 +19,46 @@
             return "#A45600"
         if self == GyroColor.COBALT:
             return "#56789D"
         if self == GyroColor.CRIMSON:
             return "#FF6562"
         if self == GyroColor.EMERALD:
             return "#4E9761"
-    
+
     @property
     def text(self) -> str:
         return f"&push;&main-color={self.color};{self.name}&pop;"
 
-GYRO_STATES = ["IS00", "IS01", "IS02", "IS03"]
+GYRO_STATES = [
+    State.InternalState00,
+    State.InternalState01,
+    State.InternalState02,
+    State.InternalState03,
+]
 
 
 def randomize_minigyro_chamber(editor: PatcherEditor, rng: random.Random):
     mrea = editor.get_mrea(MINIGYRO_CHAMBER_MREA)
     solution = [GyroColor.AMBER, GyroColor.COBALT, GyroColor.CRIMSON, GyroColor.EMERALD]
     rng.shuffle(solution)
 
     counter = mrea.get_instance_by_name("Stage gate activator")
     stage_gates = [mrea.get_instance_by_name(f"Stage gate {i+1}") for i in range(4)]
 
     for i, gate in enumerate(stage_gates):
         counter.remove_connections(gate)
         for j, gyro in enumerate(solution):
-            message = "ACTV" if i == gyro.value else "DCTV"
+            message = Message.Activate if i == gyro.value else Message.Deactivate
             counter.add_connection(GYRO_STATES[j], message, gate)
-    
+
     # play jingle on the final gyro
     stop_gyros = [mrea.get_instance_by_name(f"[IN/OUT] Stop gyroscope {i+1}") for i in range(4)]
     jingle = mrea.get_instance_by_name(f"StreamedAudio - Event Jingle")
 
     stop_gyros[3].remove_connections(jingle)
-    stop_gyros[solution[3].value].add_connection("ZERO", "PLAY", jingle)
-    
+    stop_gyros[solution[3].value].add_connection(State.Zero, Message.Play, jingle)
+
     # print([f"{mrea.get_instance(c.target).name} - {c.state}: {c.message}" for c in counter.connections])
-    
+
     scan = editor.get_file(0xFBFF349D, Strg)
     solution_text = '\n'.join((gyro.text for gyro in solution))
     scan.set_string(1, f"Safety lockdown code is as follows:\n\n\n{solution_text}")
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/rubiks.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/small_randomizations/rubiks.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import random
 
 from retro_data_structures.properties.echoes.objects.Actor import Actor
 from retro_data_structures.crc import crc32
 from retro_data_structures.formats.cmdl import Cmdl
 from retro_data_structures.base_resource import RawResource
 from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MAIN_GYRO_CHAMBER_MREA
+from retro_data_structures.enums.echoes import State, Message
 
 from open_prime_rando.patcher_editor import PatcherEditor
 
 
 RUBIKS_CUBES = {
     "Puzzle 1": [
         0x240013, 0x2401A4, 0x240145,
@@ -25,15 +26,15 @@
     ]
 }
 
 
 @dataclass(frozen=True)
 class RubiksColor:
     name: str
-    state: str
+    state: State
     cmdl: int
     old_txtr: int
 
     @property
     def txtr_name(self) -> str:
         return f"rubiks_{self.name.lower()}.TXTR"
 
@@ -44,36 +45,36 @@
             data=Path(__file__).parent.parent.joinpath("custom_assets", "rubiks", self.txtr_name).read_bytes()
         )
 
 
 COLORS = {
     "RED": RubiksColor(
         name="red",
-        state="IS00",
+        state=State.InternalState00,
         cmdl=0xF21AB8BF,
         old_txtr=0x29A5FF4B,
     ),
     "GREEN": RubiksColor(
         name="green",
-        state="IS01",
+        state=State.InternalState01,
         cmdl=0x5F2ADFC3,
         old_txtr=0xEE2889A3,
     ),
     "BLUE": RubiksColor(
         name="blue",
-        state="IS02",
+        state=State.InternalState02,
         cmdl=0x8F25F715,
         old_txtr=0xFED23B81,
     )
 }
 
 
 def randomize_rubiks_puzzles(editor: PatcherEditor, rng: random.Random):
     mrea = editor.get_mrea(MAIN_GYRO_CHAMBER_MREA)
-    
+
     # Add custom textures so colorblind players can distinguish the cubes
     for color in COLORS.values():
         txtr_id = editor.add_file(color.txtr_name, color.txtr, editor.find_paks(MAIN_GYRO_CHAMBER_MREA))
 
         cmdl = editor.get_file(color.cmdl, Cmdl)
         file_ids = cmdl.raw.material_sets[0].texture_file_ids
         old_txtr = file_ids.index(color.old_txtr)
@@ -89,12 +90,12 @@
 
         puzzle = mrea.get_instance_by_name(puzzle_name)
         for color, cube_id in zip(solution, cubes):
             cube = mrea.get_instance(cube_id)
             assert cube is not None
 
             puzzle.remove_connections(cube)
-            puzzle.add_connection(color.state, "ATCH", cube)
+            puzzle.add_connection(color.state, Message.Attach, cube)
+
+            with cube.edit_properties(Actor) as props:
+                props.model = color.cmdl
 
-            props = cube.get_properties_as(Actor)
-            props.model = color.cmdl
-            cube.set_properties(props)
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/echoes/specific_area_patches.py` & `open-prime-rando-0.6.0/open_prime_rando/echoes/specific_area_patches.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from open_prime_rando.echoes.asset_ids.world import TORVUS_BOG_MLVL
 from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.formats.script_object import ScriptInstanceHelper
 from retro_data_structures.game_check import Game
 from retro_data_structures.properties.echoes.objects.Counter import Counter
 from retro_data_structures.properties.echoes.objects.Relay import Relay
 from retro_data_structures.properties.echoes.objects.ScriptLayerController import ScriptLayerController
+from retro_data_structures.enums.echoes import State, Message
 
 LOG = logging.getLogger("echoes_patcher")
 
 
 def specific_patches(editor: PatcherEditor, area_patches: dict):
     # sand_mining(editor)
     # torvus_generator(editor)
@@ -65,16 +66,16 @@
     layer_cont1 = create_layer_controller(0x9A2ACAFD, 3)
     layer_cont2 = create_layer_controller(0x9A2ACAFD, 3)
 
     # TODO: add new layers
     # TODO: add new objects to new layers
 
     obj = area.get_instance(2686994)
-    obj.add_connection("Zero", "Increment", layer_cont1)
-    obj.add_connection("Zero", "Increment", layer_cont2)
+    obj.add_connection(State.Zero, Message.Increment, layer_cont1)
+    obj.add_connection(State.Zero, Message.Increment, layer_cont2)
 
 
 def torvus_temple_crash(editor: PatcherEditor):
     """
     Remove cosmetic objects from Torvus Temple to minimize the chance of chance via alloc failure
     """
     world = editor.get_mlvl(TORVUS_BOG_MLVL)
@@ -117,11 +118,10 @@
         relay.set_properties(properties)
 
     """
     Set the destroyed cork counter to expect only one cork to be destroyed
     """
     counter = area.get_instance(0x12044E)
 
-    properties = counter.get_properties_as(Counter)
-    properties.editor_properties.unknown = 1
-    properties.max_count = 1
-    counter.set_properties(properties)
+    with counter.edit_properties(Counter) as props:
+        props.editor_properties.unknown = 1
+        props.max_count = 1
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando/p1r_patcher.py` & `open-prime-rando-0.6.0/open_prime_rando/p1r_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/patcher_editor.py` & `open-prime-rando-0.6.0/open_prime_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando/validator_with_default.py` & `open-prime-rando-0.6.0/open_prime_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/open_prime_rando.egg-info/PKG-INFO` & `open-prime-rando-0.6.0/open_prime_rando.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.5.0
+Version: 0.6.0
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Home-page: https://github.com/randovania/open-prime-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `open-prime-rando-0.5.0/open_prime_rando.egg-info/SOURCES.txt` & `open-prime-rando-0.6.0/open_prime_rando.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 open_prime_rando.egg-info/dependency_links.txt
 open_prime_rando.egg-info/entry_points.txt
 open_prime_rando.egg-info/not-zip-safe
 open_prime_rando.egg-info/requires.txt
 open_prime_rando.egg-info/top_level.txt
 open_prime_rando/__pyinstaller/__init__.py
 open_prime_rando/__pyinstaller/hook-open_prime_rando.py
-open_prime_rando/echoes/auto_enabled_elevator_patches.py
 open_prime_rando/echoes/custom_assets.py
 open_prime_rando/echoes/schema.json
 open_prime_rando/echoes/specific_area_patches.py
+open_prime_rando/echoes/vulnerabilities.py
 open_prime_rando/echoes/asset_ids/__init__.py
 open_prime_rando/echoes/asset_ids/agon_wastes.py
 open_prime_rando/echoes/asset_ids/frontend.py
 open_prime_rando/echoes/asset_ids/great_temple.py
 open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
 open_prime_rando/echoes/asset_ids/m02_spires.py
 open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
@@ -51,14 +51,17 @@
 open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
 open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
 open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
 open_prime_rando/echoes/dock_lock_rando/__init__.py
 open_prime_rando/echoes/dock_lock_rando/dock_type.py
 open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
 open_prime_rando/echoes/dock_lock_rando/map_icons.py
+open_prime_rando/echoes/elevators/__init__.py
+open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
+open_prime_rando/echoes/elevators/elevator_rando.py
 open_prime_rando/echoes/inverted/__init__.py
 open_prime_rando/echoes/inverted/area_pairs.py
 open_prime_rando/echoes/small_randomizations/__init__.py
 open_prime_rando/echoes/small_randomizations/echo_locks.py
 open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
 open_prime_rando/echoes/small_randomizations/rubiks.py
 open_prime_rando/prime_remastered/schema.json
```

### Comparing `open-prime-rando-0.5.0/setup.cfg` & `open-prime-rando-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/tests/test_echoes_custom_Assets.py` & `open-prime-rando-0.6.0/tests/test_echoes_custom_Assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.5.0/tools/asset_id_files.py` & `open-prime-rando-0.6.0/tools/asset_id_files.py`

 * *Files identical despite different names*

