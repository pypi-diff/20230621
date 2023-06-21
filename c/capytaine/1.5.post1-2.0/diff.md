# Comparing `tmp/capytaine-1.5.post1.tar.gz` & `tmp/capytaine-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capytaine-1.5.post1.tar", last modified: Tue Dec 13 15:30:06 2022, max compression
+gzip compressed data, was "capytaine-2.0.tar", last modified: Wed Jun 21 08:17:29 2023, max compression
```

## Comparing `capytaine-1.5.post1.tar` & `capytaine-2.0.tar`

### file list

```diff
@@ -1,95 +1,187 @@
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.467954 capytaine-1.5.post1/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    35147 2022-03-15 08:41:25.000000 capytaine-1.5.post1/LICENSE
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      306 2022-12-13 15:30:06.467954 capytaine-1.5.post1/PKG-INFO
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     1894 2022-11-03 11:28:14.000000 capytaine-1.5.post1/README.md
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.459954 capytaine-1.5.post1/capytaine/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      345 2022-12-13 15:30:02.000000 capytaine-1.5.post1/capytaine/__about__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     1624 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/__init__.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/bem/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)        0 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/bem/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     2938 2022-11-09 14:06:55.000000 capytaine-1.5.post1/capytaine/bem/airy_waves.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    11438 2022-12-12 14:55:05.000000 capytaine-1.5.post1/capytaine/bem/engines.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    15743 2022-11-09 14:06:55.000000 capytaine-1.5.post1/capytaine/bem/problems_and_results.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    10600 2022-11-09 14:06:55.000000 capytaine-1.5.post1/capytaine/bem/solver.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/bodies/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      156 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/bodies/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    43927 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/bodies/bodies.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      459 2022-12-07 14:32:20.000000 capytaine-1.5.post1/capytaine/bodies/dofs.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/bodies/predefined/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      376 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/bodies/predefined/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     5634 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/bodies/predefined/cylinders.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     4473 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/bodies/predefined/rectangles.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     2600 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/bodies/predefined/spheres.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/green_functions/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      107 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/green_functions/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      457 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/green_functions/abstract_green_function.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     9949 2022-12-07 14:32:20.000000 capytaine-1.5.post1/capytaine/green_functions/delhommeau.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.459954 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    11501 2022-12-07 14:32:27.000000 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/Delhommeau_integrals.f90
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     5704 2022-12-07 14:32:27.000000 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/Green_Rankine.f90
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    11936 2022-12-07 14:32:27.000000 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/Green_wave.f90
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      422 2022-12-07 14:32:27.000000 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/constants.f90
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      127 2022-12-07 14:32:27.000000 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/float32.f90
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      127 2022-12-07 14:32:27.000000 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/float64.f90
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     9529 2022-12-07 14:32:27.000000 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/matrices.f90
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    13801 2022-12-07 14:32:27.000000 capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/old_Prony_decomposition.f90
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/io/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)        0 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/io/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     6671 2022-06-14 13:45:38.000000 capytaine-1.5.post1/capytaine/io/bemio.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    11062 2022-11-03 11:28:14.000000 capytaine-1.5.post1/capytaine/io/legacy.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    28397 2022-12-12 15:43:53.000000 capytaine-1.5.post1/capytaine/io/mesh_loaders.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    19276 2022-12-12 15:43:53.000000 capytaine-1.5.post1/capytaine/io/mesh_writers.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     1431 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/io/meshio.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    18234 2022-11-03 11:28:14.000000 capytaine-1.5.post1/capytaine/io/xarray.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/matrices/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      742 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/matrices/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    24454 2022-12-07 14:32:20.000000 capytaine-1.5.post1/capytaine/matrices/block.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    12968 2022-12-07 14:32:20.000000 capytaine-1.5.post1/capytaine/matrices/block_toeplitz.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     3158 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/matrices/builders.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     6316 2022-12-07 14:32:20.000000 capytaine-1.5.post1/capytaine/matrices/linear_solvers.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    15926 2022-12-07 14:32:20.000000 capytaine-1.5.post1/capytaine/matrices/low_rank.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/meshes/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      399 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/meshes/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    18700 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/meshes/clipper.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     9979 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/meshes/collections.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    12718 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/meshes/geometry.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    31588 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/meshes/meshes.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine/meshes/predefined/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      381 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/meshes/predefined/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    12472 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/meshes/predefined/cylinders.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    10856 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/meshes/predefined/rectangles.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     1643 2022-12-12 15:12:48.000000 capytaine-1.5.post1/capytaine/meshes/predefined/spheres.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     6909 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/meshes/properties.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    14257 2022-11-03 11:28:14.000000 capytaine-1.5.post1/capytaine/meshes/quality.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     6265 2022-12-12 15:12:49.000000 capytaine-1.5.post1/capytaine/meshes/surface_integrals.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    13539 2022-12-12 15:12:49.000000 capytaine-1.5.post1/capytaine/meshes/symmetric.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.467954 capytaine-1.5.post1/capytaine/post_pro/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      274 2022-11-03 11:28:14.000000 capytaine-1.5.post1/capytaine/post_pro/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     3201 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/post_pro/free_surfaces.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     3352 2022-11-03 11:28:14.000000 capytaine-1.5.post1/capytaine/post_pro/impedance.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     1722 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/post_pro/kochin.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     2201 2022-11-03 11:28:14.000000 capytaine-1.5.post1/capytaine/post_pro/rao.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.467954 capytaine-1.5.post1/capytaine/tools/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)        0 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/tools/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     1348 2022-12-12 14:41:16.000000 capytaine-1.5.post1/capytaine/tools/lru_cache.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      898 2022-11-03 11:28:14.000000 capytaine-1.5.post1/capytaine/tools/optional_imports.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     2731 2022-11-03 11:28:14.000000 capytaine-1.5.post1/capytaine/tools/prony_decomposition.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.467954 capytaine-1.5.post1/capytaine/ui/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)        0 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/ui/__init__.py
--rwxrwxr-x   0 mancellin  (1000) mancellin  (1000)     1549 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/ui/cli.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.467954 capytaine-1.5.post1/capytaine/ui/vtk/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      200 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/ui/vtk/__init__.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    13317 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/ui/vtk/animation.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      981 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/ui/vtk/body_viewer.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     2679 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/ui/vtk/helpers.py
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)    14789 2022-05-17 12:47:21.000000 capytaine-1.5.post1/capytaine/ui/vtk/mesh_viewer.py
-drwxrwxr-x   0 mancellin  (1000) mancellin  (1000)        0 2022-12-13 15:30:06.463954 capytaine-1.5.post1/capytaine.egg-info/
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      306 2022-12-13 15:30:06.000000 capytaine-1.5.post1/capytaine.egg-info/PKG-INFO
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     2560 2022-12-13 15:30:06.000000 capytaine-1.5.post1/capytaine.egg-info/SOURCES.txt
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)        1 2022-12-13 15:30:06.000000 capytaine-1.5.post1/capytaine.egg-info/dependency_links.txt
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)       52 2022-12-13 15:30:06.000000 capytaine-1.5.post1/capytaine.egg-info/entry_points.txt
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)      324 2022-12-13 15:30:06.000000 capytaine-1.5.post1/capytaine.egg-info/requires.txt
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)       10 2022-12-13 15:30:06.000000 capytaine-1.5.post1/capytaine.egg-info/top_level.txt
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)       38 2022-12-13 15:30:06.467954 capytaine-1.5.post1/setup.cfg
--rw-rw-r--   0 mancellin  (1000) mancellin  (1000)     3920 2022-12-13 15:12:05.000000 capytaine-1.5.post1/setup.py
+-rw-rw-r--   0        0        0     1723 1970-01-01 00:00:00.000000 capytaine-2.0/.github/workflows/build_wheels.yaml
+-rw-rw-r--   0        0        0     1127 1970-01-01 00:00:00.000000 capytaine-2.0/.github/workflows/tests.yaml
+-rw-rw-r--   0        0        0     2072 1970-01-01 00:00:00.000000 capytaine-2.0/.gitignore
+-rw-rw-r--   0        0        0     1471 1970-01-01 00:00:00.000000 capytaine-2.0/.zenodo.json
+-rw-rw-r--   0        0        0     2284 1970-01-01 00:00:00.000000 capytaine-2.0/CONTRIBUTING.md
+-rw-rw-r--   0        0        0      341 1970-01-01 00:00:00.000000 capytaine-2.0/Dockerfile
+-rw-rw-r--   0        0        0    35147 1970-01-01 00:00:00.000000 capytaine-2.0/LICENSE
+-rw-rw-r--   0        0        0      565 1970-01-01 00:00:00.000000 capytaine-2.0/Makefile
+-rw-rw-r--   0        0        0     2005 1970-01-01 00:00:00.000000 capytaine-2.0/README.md
+-rwxrwxr-x   0        0        0      412 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/__about__.py
+-rw-rw-r--   0        0        0     1617 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/__init__.py
+-rw-rw-r--   0        0        0        0 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bem/__init__.py
+-rw-rw-r--   0        0        0     3266 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bem/airy_waves.py
+-rw-rw-r--   0        0        0    12290 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bem/engines.py
+-rw-rw-r--   0        0        0    18126 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bem/problems_and_results.py
+-rw-rw-r--   0        0        0    15139 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bem/solver.py
+-rw-rw-r--   0        0        0      156 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bodies/__init__.py
+-rw-rw-r--   0        0        0    43728 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bodies/bodies.py
+-rw-rw-r--   0        0        0      598 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bodies/dofs.py
+-rw-rw-r--   0        0        0      376 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bodies/predefined/__init__.py
+-rw-rw-r--   0        0        0     5634 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bodies/predefined/cylinders.py
+-rw-rw-r--   0        0        0     4473 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bodies/predefined/rectangles.py
+-rw-rw-r--   0        0        0     2600 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/bodies/predefined/spheres.py
+-rw-rw-r--   0        0        0      107 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/__init__.py
+-rw-rw-r--   0        0        0      457 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/abstract_green_function.py
+-rw-rw-r--   0        0        0    11942 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/delhommeau.py
+-rw-rw-r--   0        0        0       30 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/.gitignore
+-rw-rw-r--   0        0        0    11359 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/LICENSE
+-rw-rw-r--   0        0        0     2877 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/Makefile
+-rw-rw-r--   0        0        0     1101 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/README.md
+-rw-rw-r--   0        0        0     8469 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/benchmarks/openmp/benchmark_omp.f90
+-rw-rw-r--   0        0        0      203 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/benchmarks/openmp/display_mesh.py
+-rw-rw-r--   0        0        0     2711 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/benchmarks/openmp/read_output.py
+-rw-rw-r--   0        0        0     8053 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/benchmarks/profiling/benchmark_profiling.f90
+-rw-rw-r--   0        0        0     2756 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/benchmarks/tabulations/benchmark_tabulation.f90
+-rw-rw-r--   0        0        0     7586 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/examples/minimal/minimal_example.f90
+-rw-rw-r--   0        0        0     1740 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/examples/minimal/minimal_example.py
+-rw-rw-r--   0        0        0    11501 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/src/Delhommeau_integrals.f90
+-rw-rw-r--   0        0        0     5729 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/src/Green_Rankine.f90
+-rw-rw-r--   0        0        0    12013 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/src/Green_wave.f90
+-rw-rw-r--   0        0        0      422 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/src/constants.f90
+-rw-rw-r--   0        0        0      127 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/src/float32.f90
+-rw-rw-r--   0        0        0      127 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/src/float64.f90
+-rw-rw-r--   0        0        0    10340 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/src/matrices.f90
+-rw-rw-r--   0        0        0    13801 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libDelhommeau/src/old_Prony_decomposition.f90
+-rw-rw-r--   0        0        0        0 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/green_functions/libs/__init__.py
+-rw-rw-r--   0        0        0        0 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/io/__init__.py
+-rw-rw-r--   0        0        0     6603 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/io/bemio.py
+-rw-rw-r--   0        0        0    13697 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/io/legacy.py
+-rw-rw-r--   0        0        0    30660 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/io/mesh_loaders.py
+-rw-rw-r--   0        0        0    21132 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/io/mesh_writers.py
+-rw-rw-r--   0        0        0     1431 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/io/meshio.py
+-rw-rw-r--   0        0        0    20282 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/io/xarray.py
+-rw-rw-r--   0        0        0      742 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/matrices/__init__.py
+-rw-rw-r--   0        0        0    24519 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/matrices/block.py
+-rw-rw-r--   0        0        0    12968 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/matrices/block_toeplitz.py
+-rw-rw-r--   0        0        0     3158 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/matrices/builders.py
+-rw-rw-r--   0        0        0     6313 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/matrices/linear_solvers.py
+-rw-rw-r--   0        0        0    15917 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/matrices/low_rank.py
+-rw-rw-r--   0        0        0      399 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/__init__.py
+-rw-rw-r--   0        0        0    18702 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/clipper.py
+-rw-rw-r--   0        0        0     9604 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/collections.py
+-rw-rw-r--   0        0        0    14159 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/geometry.py
+-rw-rw-r--   0        0        0    27769 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/meshes.py
+-rw-rw-r--   0        0        0      381 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/predefined/__init__.py
+-rw-rw-r--   0        0        0    12472 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/predefined/cylinders.py
+-rw-rw-r--   0        0        0    10856 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/predefined/rectangles.py
+-rw-rw-r--   0        0        0     1643 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/predefined/spheres.py
+-rw-rw-r--   0        0        0     7665 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/properties.py
+-rw-rw-r--   0        0        0    14421 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/quality.py
+-rw-rw-r--   0        0        0     2264 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/surface_integrals.py
+-rw-rw-r--   0        0        0    13539 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/meshes/symmetric.py
+-rw-rw-r--   0        0        0      274 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/post_pro/__init__.py
+-rw-rw-r--   0        0        0     3201 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/post_pro/free_surfaces.py
+-rw-rw-r--   0        0        0     3385 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/post_pro/impedance.py
+-rw-rw-r--   0        0        0     1728 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/post_pro/kochin.py
+-rw-rw-r--   0        0        0     2622 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/post_pro/rao.py
+-rw-rw-r--   0        0        0        0 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/tools/__init__.py
+-rw-rw-r--   0        0        0      810 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/tools/deprecation_handling.py
+-rw-rw-r--   0        0        0     1380 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/tools/lists_of_points.py
+-rw-rw-r--   0        0        0     1348 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/tools/lru_cache.py
+-rw-rw-r--   0        0        0      898 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/tools/optional_imports.py
+-rw-rw-r--   0        0        0     2731 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/tools/prony_decomposition.py
+-rw-rw-r--   0        0        0        0 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/ui/__init__.py
+-rwxrwxr-x   0        0        0     1549 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/ui/cli.py
+-rw-rw-r--   0        0        0      200 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/ui/vtk/__init__.py
+-rw-rw-r--   0        0        0    11461 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/ui/vtk/animation.py
+-rw-rw-r--   0        0        0      981 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/ui/vtk/body_viewer.py
+-rw-rw-r--   0        0        0     2679 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/ui/vtk/helpers.py
+-rw-rw-r--   0        0        0    14789 1970-01-01 00:00:00.000000 capytaine-2.0/capytaine/ui/vtk/mesh_viewer.py
+-rw-rw-r--   0        0        0     1173 1970-01-01 00:00:00.000000 capytaine-2.0/docs/Makefile
+-rw-rw-r--   0        0        0      319 1970-01-01 00:00:00.000000 capytaine-2.0/docs/_static/custom.css
+-rw-rw-r--   0        0        0      512 1970-01-01 00:00:00.000000 capytaine-2.0/docs/_static/proof.css
+-rw-rw-r--   0        0        0      344 1970-01-01 00:00:00.000000 capytaine-2.0/docs/_static/proof.js
+-rw-rw-r--   0        0        0      182 1970-01-01 00:00:00.000000 capytaine-2.0/docs/_templates/layout.html
+-rw-rw-r--   0        0        0    32067 1970-01-01 00:00:00.000000 capytaine-2.0/docs/changelog.rst
+-rw-rw-r--   0        0        0     1602 1970-01-01 00:00:00.000000 capytaine-2.0/docs/citing.rst
+-rw-rw-r--   0        0        0     6063 1970-01-01 00:00:00.000000 capytaine-2.0/docs/conf.py
+-rw-rw-r--   0        0        0      138 1970-01-01 00:00:00.000000 capytaine-2.0/docs/developer_manual/index.rst
+-rw-rw-r--   0        0        0     6035 1970-01-01 00:00:00.000000 capytaine-2.0/docs/developer_manual/installation.rst
+-rw-rw-r--   0        0        0     4645 1970-01-01 00:00:00.000000 capytaine-2.0/docs/developer_manual/overview.rst
+-rw-rw-r--   0        0        0     2264 1970-01-01 00:00:00.000000 capytaine-2.0/docs/features.rst
+-rw-rw-r--   0        0        0     3325 1970-01-01 00:00:00.000000 capytaine-2.0/docs/index.rst
+-rw-rw-r--   0        0        0     2161 1970-01-01 00:00:00.000000 capytaine-2.0/docs/theory_manual/bibliography.rst
+-rw-rw-r--   0        0        0      124 1970-01-01 00:00:00.000000 capytaine-2.0/docs/theory_manual/index.rst
+-rw-rw-r--   0        0        0    24978 1970-01-01 00:00:00.000000 capytaine-2.0/docs/theory_manual/theory.rst
+-rw-rw-r--   0        0        0     2249 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/conventions.rst
+-rw-rw-r--   0        0        0     4436 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/cookbook.rst
+-rw-rw-r--   0        0        0     1790 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/Nemoh.cal
+-rw-rw-r--   0        0        0     2184 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/animate_free_surface.py
+-rw-rw-r--   0        0        0     1371 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/axisymmetric_buoy.py
+-rw-rw-r--   0        0        0    35254 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/boat_200.mar
+-rw-rw-r--   0        0        0     2974 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/boat_animation.py
+-rw-rw-r--   0        0        0     1021 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/compare_Green_functions.py
+-rw-rw-r--   0        0        0     1454 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/convergence_study.py
+-rw-rw-r--   0        0        0     2296 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/custom_Green_function.py
+-rw-rw-r--   0        0        0     1702 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/custom_dofs.py
+-rw-rw-r--   0        0        0     1706 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/finite_depth_cylinder.py
+-rw-rw-r--   0        0        0      724 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/free_surface_elevation.py
+-rw-rw-r--   0        0        0     2132 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/haskind.py
+-rw-rw-r--   0        0        0     2572 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/hydrostatics.py
+-rw-rw-r--   0        0        0     1191 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/kochin.py
+-rw-rw-r--   0        0        0     1524 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/multibody.py
+-rw-rw-r--   0        0        0      691 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/plot_influence_matrix.py
+-rw-rw-r--   0        0        0     1574 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/plot_velocity_in_domain.py
+-rw-rw-r--   0        0        0     1703 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/radiation_cylinder.py
+-rw-rw-r--   0        0        0      650 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/examples/symmetric_body.py
+-rw-rw-r--   0        0        0     5824 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/hydrostatics.rst
+-rw-rw-r--   0        0        0      240 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/index.rst
+-rw-rw-r--   0        0        0     7426 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/installation.rst
+-rw-rw-r--   0        0        0    12220 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/mesh.rst
+-rw-rw-r--   0        0        0     8332 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/outputs.rst
+-rw-rw-r--   0        0        0     5114 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/post_pro.rst
+-rw-rw-r--   0        0        0     7092 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/problem_setup.rst
+-rw-rw-r--   0        0        0     7300 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/resolution.rst
+-rw-rw-r--   0        0        0    13513 1970-01-01 00:00:00.000000 capytaine-2.0/docs/user_manual/tutorial.rst
+-rw-rw-r--   0        0        0     5084 1970-01-01 00:00:00.000000 capytaine-2.0/meson.build
+-rw-rw-r--   0        0        0      993 1970-01-01 00:00:00.000000 capytaine-2.0/pyproject.toml
+-rw-rw-r--   0        0        0   278848 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Bemio_verification_cases/sphere.out
+-rw-rw-r--   0        0        0     1606 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Hydrostatics_cases/sphere__hor_cyl__ver_cyl.pkl.json
+-rw-rw-r--   0        0        0    65058 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/Cylinder/Cylinder.dat
+-rw-rw-r--   0        0        0     2142 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/Cylinder/Nemoh.cal
+-rw-rw-r--   0        0        0     2320 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/Cylinder/Nemoh_v3.cal
+-rw-rw-r--   0        0        0      695 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/Cylinder/reference_results/DiffractionForce.tec
+-rw-rw-r--   0        0        0      695 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/Cylinder/reference_results/ExcitationForce.tec
+-rw-rw-r--   0        0        0     2860 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/Cylinder/reference_results/RadiationCoefficients.tec
+-rw-rw-r--   0        0        0     3402 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/Nemoh.m
+-rw-rw-r--   0        0        0     2199 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/NonSymmetrical/Nemoh.cal
+-rw-rw-r--   0        0        0     2367 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/NonSymmetrical/Nemoh_v3.cal
+-rw-rw-r--   0        0        0    47266 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/NonSymmetrical/NonSymmetrical.dat
+-rw-rw-r--   0        0        0     8339 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/NonSymmetrical/reference_results/DiffractionForce.tec
+-rw-rw-r--   0        0        0     8339 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/NonSymmetrical/reference_results/ExcitationForce.tec
+-rw-rw-r--   0        0        0    48724 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/Nemoh_verification_cases/NonSymmetrical/reference_results/RadiationCoefficients.tec
+-rw-rw-r--   0        0        0      114 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/io_legacy_cases/reference_data/single_body/Hydrostatics.dat
+-rw-rw-r--   0        0        0      468 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/io_legacy_cases/reference_data/single_body/KH.dat
+-rw-rw-r--   0        0        0      114 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/io_legacy_cases/reference_data/single_body_list/Hydrostatics.dat
+-rw-rw-r--   0        0        0      468 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/io_legacy_cases/reference_data/single_body_list/KH.dat
+-rw-rw-r--   0        0        0      114 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/io_legacy_cases/reference_data/two_bodies_list/Hydrostatics_0.dat
+-rw-rw-r--   0        0        0      114 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/io_legacy_cases/reference_data/two_bodies_list/Hydrostatics_1.dat
+-rw-rw-r--   0        0        0      468 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/io_legacy_cases/reference_data/two_bodies_list/KH_0.dat
+-rw-rw-r--   0        0        0      468 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/io_legacy_cases/reference_data/two_bodies_list/KH_1.dat
+-rw-rw-r--   0        0        0    21282 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/mesh_files_examples/barge.med
+-rw-rw-r--   0        0        0     4726 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bem_engines.py
+-rw-rw-r--   0        0        0     5735 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bem_green_functions.py
+-rw-rw-r--   0        0        0    10665 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bem_hierarchical_toeplitz_matrices.py
+-rw-rw-r--   0        0        0     2414 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bem_linear_combination_of_dofs.py
+-rw-rw-r--   0        0        0     9081 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bem_potential_velocity_and_free_surface_elevation.py
+-rw-rw-r--   0        0        0    14622 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bem_problems_and_results.py
+-rw-rw-r--   0        0        0     4391 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bem_solver.py
+-rw-rw-r--   0        0        0     2329 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bem_with_quadratures.py
+-rw-rw-r--   0        0        0     8877 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bodies.py
+-rw-rw-r--   0        0        0     6926 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_bodies_predefined.py
+-rw-rw-r--   0        0        0    12479 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_consistency_with_Nemoh_2.py
+-rw-rw-r--   0        0        0    18472 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_hydrostatics.py
+-rw-rw-r--   0        0        0     6732 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_io.py
+-rw-rw-r--   0        0        0     9937 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_io_meshes.py
+-rw-rw-r--   0        0        0     6807 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_linear_solvers.py
+-rw-rw-r--   0        0        0    17117 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_matrices.py
+-rw-rw-r--   0        0        0     8471 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_meshes.py
+-rw-rw-r--   0        0        0     5784 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_meshes_collections_and_symmetries.py
+-rw-rw-r--   0        0        0     5475 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_meshes_geometry.py
+-rw-rw-r--   0        0        0     8691 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_meshes_predefined.py
+-rw-rw-r--   0        0        0     3750 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_post_pro.py
+-rw-rw-r--   0        0        0     1374 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_post_pro_kochin.py
+-rw-rw-r--   0        0        0     1073 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_ui_matplotlib.py
+-rw-rw-r--   0        0        0      758 1970-01-01 00:00:00.000000 capytaine-2.0/pytest/test_ui_vtk.py
+-rw-r--r--   0        0        0    43314 1970-01-01 00:00:00.000000 capytaine-2.0/PKG-INFO
```

### Comparing `capytaine-1.5.post1/LICENSE` & `capytaine-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/README.md` & `capytaine-2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # Capytaine: a linear potential flow BEM solver with Python.
 
 [![DOI](http://joss.theoj.org/papers/10.21105/joss.01341/status.svg)](https://doi.org/10.21105/joss.01341)
+![CI status](https://github.com/capytaine/capytaine/actions/workflows/tests.yaml/badge.svg?event=push)
 
 Capytaine is Python package for the simulation of the interaction between water waves and floating bodies in frequency domain.
 It is built around a full rewrite of the open source Boundary Element Method (BEM) solver Nemoh for the linear potential flow wave theory.
 
 ## Installation
 
-On Windows, macOS and Linux, using the [Conda package manager](https://www.anaconda.com/distribution/):
+Packages for Windows, macOS and Linux are available on PyPI:
 
 ```bash
+pip install capytaine
+```
+and Conda-forge:
+```bash
 conda install -c conda-forge capytaine
 ```
 
 ## Documentation
 
 [https://ancell.in/capytaine/latest/](https://ancell.in/capytaine/latest/)
 
 ## License
 
-Copyright (C) 2017-2022, Matthieu Ancellin
+Copyright (C) 2017-2023, Matthieu Ancellin
 
 Since April 2022, the development of Capytaine is funded by the Alliance for Sustainable Energy, LLC, Managing and Operating Contractor for the National Renewable Energy Laboratory (NREL) for the U.S. Department of Energy.
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
```

### Comparing `capytaine-1.5.post1/capytaine/__init__.py` & `capytaine-2.0/capytaine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from capytaine.bodies.dofs import rigid_body_dofs
 
 from capytaine.bodies.predefined.spheres import Sphere
 from capytaine.bodies.predefined.cylinders import VerticalCylinder, HorizontalCylinder, Disk
 from capytaine.bodies.predefined.rectangles import Rectangle, RectangularParallelepiped, OpenRectangularParallelepiped
 
 from capytaine.bem.problems_and_results import RadiationProblem, DiffractionProblem
-from capytaine.bem.solver import Nemoh, BEMSolver
+from capytaine.bem.solver import BEMSolver
 from capytaine.bem.engines import BasicMatrixEngine, HierarchicalToeplitzMatrixEngine
 from capytaine.green_functions.delhommeau import Delhommeau, XieDelhommeau
 
 from capytaine.post_pro.free_surfaces import FreeSurface
 
 from capytaine.io.mesh_loaders import load_mesh
 from capytaine.io.xarray import assemble_dataset
```

### Comparing `capytaine-1.5.post1/capytaine/bem/engines.py` & `capytaine-2.0/capytaine/bem/engines.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 #  ABSTRACT CLASS  #
 ####################
 
 class MatrixEngine(ABC):
     """Abstract method to build a matrix."""
 
     @abstractmethod
-    def build_matrices(self, mesh1, mesh2, free_surface, sea_bottom, wavenumber, green_function):
+    def build_matrices(self, mesh1, mesh2, free_surface, water_depth, wavenumber, green_function):
         pass
 
     def build_S_matrix(self, *args, **kwargs):
         """Similar to :code:`build_matrices`, but returning only :math:`S`"""
         S, _ = self.build_matrices(*args, **kwargs)  # Could be optimized...
         return S
 
@@ -75,26 +75,37 @@
 
         self.exportable_settings = {
             'engine': 'BasicMatrixEngine',
             'matrix_cache_size': matrix_cache_size,
             'linear_solver': str(linear_solver),
         }
 
-    def build_matrices(self, mesh1, mesh2, free_surface, sea_bottom, wavenumber, green_function):
+    def __str__(self):
+        params = f"linear_solver=\'{self.exportable_settings['linear_solver']}\'"
+        params += f", matrix_cache_size={self.exportable_settings['matrix_cache_size']}" if self.exportable_settings['matrix_cache_size'] != 1 else ""
+        return f"BasicMatrixEngine({params})"
+
+    def __repr__(self):
+        return self.__str__()
+
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__str__())
+
+    def build_matrices(self, mesh1, mesh2, free_surface, water_depth, wavenumber, green_function):
         r"""Build the influence matrices between mesh1 and mesh2.
 
         Parameters
         ----------
         mesh1: Mesh or CollectionOfMeshes
             mesh of the receiving body (where the potential is measured)
         mesh2: Mesh or CollectionOfMeshes
             mesh of the source body (over which the source distribution is integrated)
         free_surface: float
             position of the free surface (default: :math:`z = 0`)
-        sea_bottom: float
+        water_depth: float
             position of the sea bottom (default: :math:`z = -\infty`)
         wavenumber: float
             wavenumber (default: 1.0)
         green_function: AbstractGreenFunction
             object with an "evaluate" method that computes the Green function.
 
         Returns
@@ -104,25 +115,25 @@
         """
 
         if (isinstance(mesh1, ReflectionSymmetricMesh)
                 and isinstance(mesh2, ReflectionSymmetricMesh)
                 and mesh1.plane == mesh2.plane):
 
             S_a, V_a = self.build_matrices(
-                mesh1[0], mesh2[0], free_surface, sea_bottom, wavenumber,
+                mesh1[0], mesh2[0], free_surface, water_depth, wavenumber,
                 green_function)
             S_b, V_b = self.build_matrices(
-                mesh1[0], mesh2[1], free_surface, sea_bottom, wavenumber,
+                mesh1[0], mesh2[1], free_surface, water_depth, wavenumber,
                 green_function)
 
             return BlockSymmetricToeplitzMatrix([[S_a, S_b]]), BlockSymmetricToeplitzMatrix([[V_a, V_b]])
 
         else:
             return green_function.evaluate(
-                mesh1, mesh2, free_surface, sea_bottom, wavenumber,
+                mesh1, mesh2, free_surface, water_depth, wavenumber,
             )
 
 ###################################
 #  HIERARCHIAL TOEPLITZ MATRICES  #
 ###################################
 
 class HierarchicalToeplitzMatrixEngine(MatrixEngine):
@@ -152,16 +163,26 @@
         self.exportable_settings = {
             'engine': 'HierarchicalToeplitzMatrixEngine',
             'ACA_distance': ACA_distance,
             'ACA_tol': ACA_tol,
             'matrix_cache_size': matrix_cache_size,
         }
 
+    def __str__(self):
+        params = f"ACA_distance={self.ACA_distance}"
+        params += f", ACA_tol={self.ACA_tol}"
+        params += f", matrix_cache_size={self.exportable_settings['matrix_cache_size']}" if self.exportable_settings['matrix_cache_size'] != 1 else ""
+        return f"HierarchicalToeplitzMatrixEngine({params})"
+
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__str__())
+
+
     def build_matrices(self,
-                       mesh1, mesh2, free_surface, sea_bottom, wavenumber, green_function,
+                       mesh1, mesh2, free_surface, water_depth, wavenumber, green_function,
                        _rec_depth=1):
         """Recursively builds a hierarchical matrix between mesh1 and mesh2.
         
         Same arguments as :func:`BasicMatrixEngine.build_matrices`.
 
         :code:`_rec_depth` keeps track of the recursion depth only for pretty log printing.
         """
@@ -184,39 +205,39 @@
         if (isinstance(mesh1, ReflectionSymmetricMesh)
                 and isinstance(mesh2, ReflectionSymmetricMesh)
                 and mesh1.plane == mesh2.plane):
 
             LOG.debug(log_entry + " using mirror symmetry.")
 
             S_a, V_a = self.build_matrices(
-                mesh1[0], mesh2[0], free_surface, sea_bottom, wavenumber, green_function,
+                mesh1[0], mesh2[0], free_surface, water_depth, wavenumber, green_function,
                 _rec_depth=_rec_depth+1)
             S_b, V_b = self.build_matrices(
-                mesh1[0], mesh2[1], free_surface, sea_bottom, wavenumber, green_function,
+                mesh1[0], mesh2[1], free_surface, water_depth, wavenumber, green_function,
                 _rec_depth=_rec_depth+1)
 
             return BlockSymmetricToeplitzMatrix([[S_a, S_b]]), BlockSymmetricToeplitzMatrix([[V_a, V_b]])
 
         elif (isinstance(mesh1, TranslationalSymmetricMesh)
               and isinstance(mesh2, TranslationalSymmetricMesh)
               and np.allclose(mesh1.translation, mesh2.translation)
               and mesh1.nb_submeshes == mesh2.nb_submeshes):
 
             LOG.debug(log_entry + " using translational symmetry.")
 
             S_list, V_list = [], []
             for submesh in mesh2:
                 S, V = self.build_matrices(
-                    mesh1[0], submesh, free_surface, sea_bottom, wavenumber, green_function,
+                    mesh1[0], submesh, free_surface, water_depth, wavenumber, green_function,
                     _rec_depth=_rec_depth+1)
                 S_list.append(S)
                 V_list.append(V)
             for submesh in mesh1[1:][::-1]:
                 S, V = self.build_matrices(
-                    submesh, mesh2[0], free_surface, sea_bottom, wavenumber, green_function,
+                    submesh, mesh2[0], free_surface, water_depth, wavenumber, green_function,
                     _rec_depth=_rec_depth+1)
                 S_list.append(S)
                 V_list.append(V)
 
             return BlockToeplitzMatrix([S_list]), BlockToeplitzMatrix([V_list])
 
         elif (isinstance(mesh1, AxialSymmetricMesh)
@@ -225,15 +246,15 @@
               and mesh1.nb_submeshes == mesh2.nb_submeshes):
 
             LOG.debug(log_entry + " using rotation symmetry.")
 
             S_line, V_line = [], []
             for submesh in mesh2[:mesh2.nb_submeshes]:
                 S, V = self.build_matrices(
-                    mesh1[0], submesh, free_surface, sea_bottom, wavenumber, green_function,
+                    mesh1[0], submesh, free_surface, water_depth, wavenumber, green_function,
                     _rec_depth=_rec_depth+1)
                 S_line.append(S)
                 V_line.append(V)
 
             return BlockCirculantMatrix([S_line]), BlockCirculantMatrix([V_line])
 
         # I-ii) LOW-RANK MATRIX WITH ACA
@@ -241,22 +262,22 @@
         elif distance > self.ACA_distance*mesh1.diameter_of_nodes or distance > self.ACA_distance*mesh2.diameter_of_nodes:
 
             LOG.debug(log_entry + " using ACA.")
 
             def get_row_func(i):
                 s, v = green_function.evaluate(
                     mesh1.extract_one_face(i), mesh2,
-                    free_surface, sea_bottom, wavenumber
+                    free_surface, water_depth, wavenumber
                 )
                 return s.flatten(), v.flatten()
 
             def get_col_func(j):
                 s, v = green_function.evaluate(
                     mesh1, mesh2.extract_one_face(j),
-                    free_surface, sea_bottom, wavenumber
+                    free_surface, water_depth, wavenumber
                 )
                 return s.flatten(), v.flatten()
 
             try:
                 return LowRankMatrix.from_rows_and_cols_functions_with_multi_ACA(
                     get_row_func, get_col_func, mesh1.nb_faces, mesh2.nb_faces,
                     nb_matrices=2, id_main=1,  # Approximate V and get an approximation of S at the same time
@@ -273,15 +294,15 @@
             LOG.debug(log_entry + " using block matrix structure.")
 
             S_matrix, V_matrix = [], []
             for submesh1 in mesh1:
                 S_line, V_line = [], []
                 for submesh2 in mesh2:
                     S, V = self.build_matrices(
-                        submesh1, submesh2, free_surface, sea_bottom, wavenumber, green_function,
+                        submesh1, submesh2, free_surface, water_depth, wavenumber, green_function,
                         _rec_depth=_rec_depth+1)
 
                     S_line.append(S)
                     V_line.append(V)
                 S_matrix.append(S_line)
                 V_matrix.append(V_line)
 
@@ -289,11 +310,11 @@
 
         # II-ii) PLAIN NUMPY ARRAY
 
         else:
             LOG.debug(log_entry)
 
             S, V = green_function.evaluate(
-                mesh1, mesh2, free_surface, sea_bottom, wavenumber,
+                mesh1, mesh2, free_surface, water_depth, wavenumber,
             )
             return S, V
```

### Comparing `capytaine-1.5.post1/capytaine/bem/problems_and_results.py` & `capytaine-2.0/capytaine/bem/problems_and_results.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,166 @@
 #!/usr/bin/env python
 # coding: utf-8
 """Definition of the problems to solve with the BEM solver, and the results of this resolution."""
-# Copyright (C) 2017-2020 Matthieu Ancellin
-# See LICENSE file at <https://github.com/mancellin/capytaine>
+# Copyright (C) 2017-2023 Matthieu Ancellin
+# See LICENSE file at <https://github.com/capytaine/capytaine>
 
 import logging
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import newton
 
+from capytaine.tools.deprecation_handling import _get_water_depth
 from capytaine.meshes.collections import CollectionOfMeshes
 from capytaine.bem.airy_waves import airy_waves_velocity, froude_krylov_force
 
 LOG = logging.getLogger(__name__)
 
 _default_parameters = {'rho': 1000.0, 'g': 9.81, 'omega': 1.0,
                       'free_surface': 0.0, 'water_depth': np.infty,
-                      'convention': "nemoh"}
+                      'wave_direction': 0.0}
 
 
 class LinearPotentialFlowProblem:
     """General class of a potential flow problem.
 
+    At most one of the following parameter must be provided: omega, period, wavenumber or wavelength.
+    Internally only omega is stored, hence setting another parameter can lead to small rounding errors.
+
     Parameters
     ----------
     body: FloatingBody, optional
         The body interacting with the waves
     free_surface: float, optional
         The position of the free surface (accepted values: 0 and np.infty)
+    water_depth: float, optional
+        The depth of water in m (default: np.infty)
     sea_bottom: float, optional
-        The position of the sea bottom
+        The position of the sea bottom (deprecated: please prefer setting water_depth)
     omega: float, optional
-        The frequency of the waves in rad/s
+        The angular frequency of the waves in rad/s
+    period: float, optional
+        The period of the waves in s
+    wavenumber: float, optional
+        The angular wave number of the waves in rad/m
+    wavelength: float, optional
+        The wave length of the waves in m
     rho: float, optional
         The density of water in kg/m3 (default: 1000.0)
     g: float, optional
         The acceleration of gravity in m/s2 (default: 9.81)
-    boundary_condition: np.ndarray of shape (body.mesh.nb_faces,)
+    boundary_condition: np.ndarray of shape (body.mesh.nb_faces,), optional
         The Neumann boundary condition on the floating body
-
-    TODO: more consistent use of free_surface and sea_bottom vs. water_depth
     """
 
     def __init__(self, *,
                  body=None,
                  free_surface=_default_parameters['free_surface'],
-                 sea_bottom=-_default_parameters['water_depth'],
-                 omega=_default_parameters['omega'],
+                 water_depth=None, sea_bottom=None,
+                 omega=None, period=None, wavenumber=None, wavelength=None,
                  rho=_default_parameters['rho'],
                  g=_default_parameters['g'],
                  boundary_condition=None):
 
         self.body = body
-        self.free_surface = free_surface
-        self.sea_bottom = sea_bottom
-        self.omega = omega
-        self.rho = rho
-        self.g = g
+        self.free_surface = float(free_surface)
+        self.rho = float(rho)
+        self.g = float(g)
+
         self.boundary_condition = boundary_condition
 
+        self.water_depth = _get_water_depth(free_surface, water_depth, sea_bottom, default_water_depth=_default_parameters["water_depth"])
+        self.omega, self.period, self.wavenumber, self.wavelength, self.provided_freq_type = \
+                self._get_frequencies(omega, period, wavenumber, wavelength)
+
         self._check_data()
 
+    def _get_frequencies(self, omega, period, wavenumber, wavelength):
+        frequency_data = dict(omega=omega, period=period, wavenumber=wavenumber, wavelength=wavelength)
+        nb_provided_frequency_data = 4 - list(frequency_data.values()).count(None)
+
+        if nb_provided_frequency_data > 1:
+            raise ValueError("Settings a problem requires at most one of the following: omega (angular frequency) OR period OR wavenumber OR wavelength.\n"
+                             "Received {} of them: {}".format(nb_provided_frequency_data, {k: v for k, v in frequency_data.items() if v is not None}))
+
+        if nb_provided_frequency_data == 0:
+            provided_freq_type = 'omega'
+            frequency_data = {'omega': _default_parameters['omega']}
+        else:
+            provided_freq_type = [k for k, v in frequency_data.items() if v is not None][0]
+
+        if frequency_data[provided_freq_type] in {0.0, np.infty}:
+            raise NotImplementedError("Zero and infinite frequencies are currently not supported.")
+
+
+        if provided_freq_type in {'omega', 'period'}:
+            if provided_freq_type == 'omega':
+                omega = frequency_data['omega']
+                period = 2*np.pi/omega
+            else:  # provided_freq_type is 'period'
+                period = frequency_data['period']
+                omega = 2*np.pi/period
+
+            if self.water_depth == np.infty:
+                wavenumber = omega**2/self.g
+            else:
+                wavenumber = newton(lambda k: k*np.tanh(k*self.water_depth) - omega**2/self.g, x0=1.0)
+            wavelength = 2*np.pi/wavenumber
+
+        else:  # provided_freq_type is 'wavelength' or 'wavenumber'
+            if provided_freq_type == 'wavelength':
+                wavelength = frequency_data['wavelength']
+                wavenumber = 2*np.pi/wavelength
+            else:  # provided_freq_type is 'wavenumber'
+                wavenumber = frequency_data['wavenumber']
+                wavelength = 2*np.pi/wavenumber
+
+            omega = np.sqrt(self.g*wavenumber*np.tanh(wavenumber*self.water_depth))
+            period = 2*np.pi/omega
+
+        return omega, period, wavenumber, wavelength, provided_freq_type
+
     def _check_data(self):
         """Sanity checks on the data."""
 
-        if self.free_surface not in [0.0, np.infty]:
+        if self.free_surface not in {0.0, np.infty}:
             raise NotImplementedError(
                 f"Free surface is {self.free_surface}. "
                 "Only z=0 and z=∞ are accepted values for the free surface position."
             )
 
-        if self.free_surface == np.infty and self.sea_bottom != -np.infty:
+        if self.free_surface == np.infty and self.water_depth != np.infty:
             raise NotImplementedError(
                 "Problems with a sea bottom but no free surface have not been implemented."
             )
 
-        if self.free_surface < self.sea_bottom:
-            raise ValueError("Sea bottom is above the free surface.")
+        if self.water_depth < 0.0:
+            raise ValueError("`water_depth` should be stricly positive.")
 
-        if self.omega in {0, np.infty} and self.depth != np.infty:
+        if self.omega in {0, np.infty} and self.water_depth != np.infty:
             raise NotImplementedError(
                 f"omega={self.omega} is only implemented for infinite depth."
             )
 
         if self.body is not None:
             if ((isinstance(self.body.mesh, CollectionOfMeshes) and len(self.body.mesh) == 0)
                     or len(self.body.mesh.faces) == 0):
                 raise ValueError(f"The mesh of the body {self.body.name} is empty.")
 
             if (any(self.body.mesh.faces_centers[:, 2] >= self.free_surface)
-                    or any(self.body.mesh.faces_centers[:, 2] <= self.sea_bottom)):
+                    or any(self.body.mesh.faces_centers[:, 2] <= -self.water_depth)):
 
                 LOG.warning(
                     f"The mesh of the body {self.body.name} is not inside the domain.\n"
-                    "Check the position of the free_surface and the sea_bottom\n"
+                    "Check the position of the free_surface and the water_depth\n"
                     "or use body.keep_immersed_part() to clip the mesh."
                 )
 
-            if self.wavelength < 8*self.body.mesh.faces_radiuses.max():
+            if self.wavelength < self.body.minimal_computable_wavelength:
                 LOG.warning(f"Mesh resolution for {self}:\n"
                         f"The resolution of the mesh '{self.body.mesh.name}' of the body '{self.body.name}' "
                         f"might be insufficient for the wavelength λ={self.wavelength:.2e}.\n"
                         f"This warning appears because the largest panel of this mesh has radius {self.body.mesh.faces_radiuses.max():.2e} > λ/8."
                         )
 
         if self.boundary_condition is not None:
@@ -119,14 +177,17 @@
     def body_name(self):
         return self.body.name if self.body is not None else 'None'
 
     def _asdict(self):
         return {"body_name": self.body_name,
                 "water_depth": self.water_depth,
                 "omega": self.omega,
+                "period": self.period,
+                "wavelength": self.wavelength,
+                "wavenumber": self.wavenumber,
                 "rho": self.rho,
                 "g": self.g}
 
     @staticmethod
     def _group_for_parallel_resolution(problems):
         """Given a list of problems, returns a list of groups of problems, such
         that each group should be executed in the same process to benefit from
@@ -136,92 +197,61 @@
         groups_of_indices = problems_params.groupby(["body_name", "water_depth", "omega", "rho", "g"]).groups.values()
         groups_of_problems = [[problems[i] for i in grp] for grp in groups_of_indices]
         return groups_of_problems
 
     def __str__(self):
         """Do not display default values in str(problem)."""
         parameters = [f"body={self.body_name}",
-                      f"omega={self.omega:.3f}",
-                      f"depth={self.depth}"]
+                      f"{self.provided_freq_type}={self.__getattribute__(self.provided_freq_type):.3f}",
+                      f"water_depth={self.water_depth}"]
         try:
             parameters.extend(self._str_other_attributes())
         except AttributeError:
             pass
 
         if not self.free_surface == _default_parameters['free_surface']:
             parameters.append(f"free_surface={self.free_surface}")
         if not self.g == _default_parameters['g']:
             parameters.append(f"g={self.g}")
         if not self.rho == _default_parameters['rho']:
             parameters.append(f"rho={self.rho}")
 
         return self.__class__.__name__ + "(" + ', '.join(parameters) + ")"
 
+    def __repr__(self):
+        return self.__str__()
+
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__str__())
+
     def _astuple(self):
-        return (self.body, self.free_surface, self.sea_bottom, self.omega, self.rho, self.g)
+        return (self.body, self.free_surface, self.water_depth,
+                self.omega, self.period, self.wavenumber, self.wavelength,
+                self.rho, self.g)
 
     def __eq__(self, other):
         if isinstance(other, LinearPotentialFlowProblem):
             return self._astuple() == other._astuple()
         else:
             return NotImplemented
 
     def __lt__(self, other):
         # Arbitrary order. Used for ordering of problems: problems with same body are grouped together.
         if isinstance(other, LinearPotentialFlowProblem):
-            return self._astuple()[:6] < other._astuple()[:6]
+            return self._astuple()[:9] < other._astuple()[:9]
             # Not the whole tuple, because when using inheriting classes,
             # "radiating_dof" cannot be compared with "wave_direction"
         else:
             return NotImplemented
 
     @property
-    def water_depth(self):
-        return self.free_surface - self.sea_bottom
-
-    @property
     def depth(self):
         return self.water_depth
 
     @property
-    def wavenumber(self):
-        if self.depth == np.infty or self.omega**2*self.depth/self.g > 20:
-            return self.omega**2/self.g
-        else:
-            return newton(lambda x: x*np.tanh(x) - self.omega**2*self.depth/self.g, x0=1.0)/self.depth
-
-    @property
-    def wavelength(self):
-        if self.wavenumber == 0.0:
-            return np.infty
-        else:
-            return 2*np.pi/self.wavenumber
-
-    @property
-    def period(self):
-        if self.omega == 0.0:
-            return np.infty
-        else:
-            return 2*np.pi/self.omega
-
-    @property
-    def dimensionless_omega(self):
-        if self.depth != np.infty:
-            return self.omega**2*self.depth/self.g
-        else:
-            raise AttributeError("Dimensionless omega is defined only for finite depth problems.")
-
-    @property
-    def dimensionless_wavenumber(self):
-        if self.depth != np.infty:
-            return self.wavenumber*self.depth
-        else:
-            raise AttributeError("Dimensionless wavenumber is defined only for finite depth problems.")
-
-    @property
     def influenced_dofs(self):
         # TODO: let the user choose the influenced dofs
         return self.body.dofs if self.body is not None else set()
 
     def make_results_container(self):
         return LinearPotentialFlowResult(self)
 
@@ -229,49 +259,46 @@
 class DiffractionProblem(LinearPotentialFlowProblem):
     """Particular LinearPotentialFlowProblem with boundary conditions
     computed from an incoming Airy wave."""
 
     def __init__(self, *,
                  body=None,
                  free_surface=_default_parameters['free_surface'],
-                 sea_bottom=-_default_parameters['water_depth'],
-                 omega=_default_parameters['omega'],
+                 water_depth=None, sea_bottom=None,
+                 omega=None, period=None, wavenumber=None, wavelength=None,
                  rho=_default_parameters['rho'],
                  g=_default_parameters['g'],
-                 wave_direction=0.0,
-                 convention=_default_parameters['convention']):
+                 wave_direction=_default_parameters['wave_direction']):
 
-        self.wave_direction = wave_direction
-        self.convention = convention
+        self.wave_direction = float(wave_direction)
 
-        super().__init__(body=body, free_surface=free_surface, sea_bottom=sea_bottom,
-                         omega=omega, rho=rho, g=g)
+        super().__init__(body=body, free_surface=free_surface, water_depth=water_depth, sea_bottom=sea_bottom,
+                         omega=omega, period=period, wavenumber=wavenumber, wavelength=wavelength, rho=rho, g=g)
 
         if not (-2*np.pi-1e-3 <= self.wave_direction <= 2*np.pi+1e-3):
             LOG.warning(f"The value {self.wave_direction} has been provided for the wave direction, and it does not look like an angle in radians. "
                          "The wave direction in Capytaine is defined in radians and not in degrees, so the result might not be what you expect. "
                          "If you were actually giving an angle in radians, use the modulo operator to give a value between -2π and 2π to disable this warning.")
 
         if self.body is not None:
 
             self.boundary_condition = -(
-                    airy_waves_velocity(self.body.mesh.faces_centers, self, convention=self.convention)
+                    airy_waves_velocity(self.body.mesh.faces_centers, self)
                     * self.body.mesh.faces_normals
             ).sum(axis=1)
 
             if len(self.body.dofs) == 0:
                 LOG.warning(f"The body {self.body.name} used in diffraction problem has no dofs!")
 
     def _astuple(self):
         return super()._astuple() + (self.wave_direction,)
 
     def _asdict(self):
         d = super()._asdict()
         d["wave_direction"] = self.wave_direction
-        d["convention"] = self.convention
         return d
 
     def _str_other_attributes(self):
         return [f"wave_direction={self.wave_direction:.3f}"]
 
     def make_results_container(self, *args, **kwargs):
         return DiffractionResult(self, *args, **kwargs)
@@ -279,24 +306,24 @@
 
 class RadiationProblem(LinearPotentialFlowProblem):
     """Particular LinearPotentialFlowProblem whose boundary conditions have
     been computed from the degree of freedom of the body."""
 
     def __init__(self, *, body=None,
                  free_surface=_default_parameters['free_surface'],
-                 sea_bottom=-_default_parameters['water_depth'],
-                 omega=_default_parameters['omega'],
+                 water_depth=None, sea_bottom=None,
+                 omega=None, period=None, wavenumber=None, wavelength=None,
                  rho=_default_parameters['rho'],
                  g=_default_parameters['g'],
                  radiating_dof=None):
 
         self.radiating_dof = radiating_dof
 
-        super().__init__(body=body, free_surface=free_surface, sea_bottom=sea_bottom,
-                         omega=omega, rho=rho, g=g)
+        super().__init__(body=body, free_surface=free_surface, water_depth=water_depth, sea_bottom=sea_bottom,
+                         omega=omega, period=period, wavenumber=wavenumber, wavelength=wavelength, rho=rho, g=g)
 
         if self.body is not None:
 
             if len(self.body.dofs) == 0:
                 raise ValueError(f"Body {self.body.name} does not have any degrees of freedom.")
 
             if self.radiating_dof is None:
@@ -305,26 +332,26 @@
             if self.radiating_dof not in self.body.dofs:
                 LOG.error(f"In {self}: the radiating degree of freedom {self.radiating_dof} is not one of"
                           f"the degrees of freedom of the body.\n"
                           f"The dofs of the body are {list(self.body.dofs.keys())}")
                 raise ValueError("Unrecognized degree of freedom name.")
 
             dof = self.body.dofs[self.radiating_dof]
-            self.boundary_condition = np.sum(dof * self.body.mesh.faces_normals, axis=1)
+            self.boundary_condition = -1j*self.omega * np.sum(dof * self.body.mesh.faces_normals, axis=1)
 
     def _astuple(self):
         return super()._astuple() + (self.radiating_dof,)
 
     def _asdict(self):
         d = super()._asdict()
         d["radiating_dof"] = self.radiating_dof
         return d
 
     def _str_other_attributes(self):
-        return [f"radiating_dof={self.radiating_dof}"]
+        return [f"radiating_dof=\'{self.radiating_dof}\'"]
 
     def make_results_container(self, *args, **kwargs):
         return RadiationResult(self, *args, **kwargs)
 
 
 class LinearPotentialFlowResult:
 
@@ -335,46 +362,48 @@
         self.potential = potential
         self.pressure = pressure
         self.fs_elevation = {}
 
         # Copy data from problem
         self.body               = self.problem.body
         self.free_surface       = self.problem.free_surface
-        self.sea_bottom         = self.problem.sea_bottom
         self.omega              = self.problem.omega
         self.rho                = self.problem.rho
         self.g                  = self.problem.g
         self.boundary_condition = self.problem.boundary_condition
         self.water_depth        = self.problem.water_depth
-        self.depth              = self.problem.depth
+        self.depth              = self.problem.water_depth
         self.wavenumber         = self.problem.wavenumber
         self.wavelength         = self.problem.wavelength
         self.period             = self.problem.period
+        self.provided_freq_type = self.problem.provided_freq_type
         self.body_name          = self.problem.body_name
         self.influenced_dofs    = self.problem.influenced_dofs
 
         if forces is not None:
             for dof in self.influenced_dofs:
                 self.store_force(dof, forces[dof])
 
     def store_force(self, dof, force):
         pass  # Implemented in sub-classes
 
     __str__ = LinearPotentialFlowProblem.__str__
+    __repr__ = LinearPotentialFlowProblem.__repr__
+    _repr_pretty_ = LinearPotentialFlowProblem._repr_pretty_
 
 
 class DiffractionResult(LinearPotentialFlowResult):
 
     def __init__(self, problem, *args, **kwargs):
         self.forces = {}
         super().__init__(problem, *args, **kwargs)
         self.wave_direction = self.problem.wave_direction
 
     def store_force(self, dof, force):
-        self.forces[dof] = 1j*self.omega*force
+        self.forces[dof] = force
 
     @property
     def records(self):
         params = self.problem._asdict()
         FK = froude_krylov_force(self.problem)
         return [dict(**params,
                      influenced_dof=dof,
@@ -388,19 +417,16 @@
     def __init__(self, problem, *args, **kwargs):
         self.added_masses = {}
         self.radiation_dampings = {}
         super().__init__(problem, *args, **kwargs)
         self.radiating_dof = self.problem.radiating_dof
 
     def store_force(self, dof, force):
-        self.added_masses[dof] = force.real
-        if self.problem.omega == np.infty:
-            self.radiation_dampings[dof] = 0
-        else:
-            self.radiation_dampings[dof] = self.problem.omega * force.imag
+        self.added_masses[dof] = force.real/self.omega**2
+        self.radiation_dampings[dof] = force.imag/self.omega
 
     @property
     def records(self):
         params = self.problem._asdict()
         return [dict(params,
                      influenced_dof=dof,
                      added_mass=self.added_masses[dof],
```

### Comparing `capytaine-1.5.post1/capytaine/bem/solver.py` & `capytaine-2.0/capytaine/bem/solver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,73 @@
-#!/usr/bin/env python
-# coding: utf-8
+# Copyright (C) 2017-2019 Matthieu Ancellin
+# See LICENSE file at <https://github.com/mancellin/capytaine>
 """Solver for the BEM problem.
 
-Example
--------
-
-::
+.. code-block:: python
 
     problem = RadiationProblem(...)
     result = BEMSolver(green_functions=..., engine=...).solve(problem)
 
 """
-# Copyright (C) 2017-2019 Matthieu Ancellin
-# See LICENSE file at <https://github.com/mancellin/capytaine>
 
 import logging
 
 import numpy as np
 
 from datetime import datetime
 
 from capytaine.bem.problems_and_results import LinearPotentialFlowProblem
 from capytaine.green_functions.delhommeau import Delhommeau
 from capytaine.bem.engines import BasicMatrixEngine, HierarchicalToeplitzMatrixEngine
 from capytaine.io.xarray import problems_from_dataset, assemble_dataset, kochin_data_array
 from capytaine.tools.optional_imports import silently_import_optional_dependency
+from capytaine.tools.lists_of_points import _normalize_points, _normalize_free_surface_points
 
 LOG = logging.getLogger(__name__)
 
 class BEMSolver:
     """
     Solver for linear potential flow problems.
 
     Parameters
     ----------
-    green_function: AbstractGreenFunction
+    green_function: AbstractGreenFunction, optional
         Object handling the computation of the Green function.
-    engine: MatrixEngine
+        (default: :class:`~capytaine.green_function.delhommeau.Delhommeau`)
+    engine: MatrixEngine, optional
         Object handling the building of matrices and the resolution of linear systems with these matrices.
+        (default: :class:`~capytaine.bem.engines.BasicMatrixEngine`)
 
     Attributes
     ----------
     exportable_settings : dict
         Settings of the solver that can be saved to reinit the same solver later.
     """
 
-    def __init__(self, *, green_function=Delhommeau(), engine=BasicMatrixEngine()):
-        self.green_function = green_function
-        self.engine = engine
+    def __init__(self, *, green_function=None, engine=None):
+        self.green_function = Delhommeau() if green_function is None else green_function
+        self.engine = BasicMatrixEngine() if engine is None else engine
 
         try:
             self.exportable_settings = {
                 **self.green_function.exportable_settings,
                 **self.engine.exportable_settings
             }
         except AttributeError:
             pass
 
+    def __str__(self):
+        return f"BEMSolver(engine={self.engine}, green_function={self.green_function})"
+
+    def __repr__(self):
+        return self.__str__()
+
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__str__())
+
     @classmethod
     def from_exported_settings(settings):
         raise NotImplementedError
 
     def solve(self, problem, keep_details=True):
         """Solve the linear potential flow problem.
 
@@ -77,23 +84,20 @@
         LinearPotentialFlowResult
             an object storing the problem data and its results
         """
         LOG.info("Solve %s.", problem)
 
         S, K = self.engine.build_matrices(
             problem.body.mesh, problem.body.mesh,
-            problem.free_surface, problem.sea_bottom, problem.wavenumber,
+            problem.free_surface, problem.water_depth, problem.wavenumber,
             self.green_function
         )
         sources = self.engine.linear_solver(K, problem.boundary_condition)
         potential = S @ sources
-        pressure = problem.rho * potential
-        # Actually, for diffraction problems: pressure over jω
-        #           for radiation problems:   pressure over -ω²
-        # The correction is done in `store_force` in the `result` object.
+        pressure = 1j * problem.omega * problem.rho * potential
 
         forces = problem.body.integrate_pressure(pressure)
 
         if not keep_details:
             result = problem.make_results_container(forces)
         else:
             result = problem.make_results_container(forces, sources, potential, pressure)
@@ -157,19 +161,133 @@
             dataset = assemble_dataset(results, attrs=attrs, **kwargs)
             dataset.update(kochin)
         else:
             results = self.solve_all(problems, keep_details=False, n_jobs=n_jobs)
             dataset = assemble_dataset(results, attrs=attrs, **kwargs)
         return dataset
 
+
+    def compute_potential(self, points, result):
+        """Compute the value of the potential at given points for a previously solved potential flow problem.
+
+        Parameters
+        ----------
+        points: array of shape (3,) or (N, 3), or 3-ple of arrays returned by meshgrid, or cpt.Mesh or cpt.CollectionOfMeshes object
+            Coordinates of the point(s) at which the potential should be computed
+        results: LinearPotentialFlowResult
+            The return of the BEM solver
+
+        Returns
+        -------
+        complex-valued array of shape (1,) or (N,) or (nx, ny, nz) or (mesh.nb_faces,) depending of the kind of input
+            The value of the potential at the points
+
+        Raises
+        ------
+        Exception: if the :code:`LinearPotentialFlowResult` object given as input does not contain the source distribution.
+        """
+        points, output_shape = _normalize_points(points, keep_mesh=True)
+        if result.sources is None:
+            raise Exception(f"""The values of the sources of {result} cannot been found.
+            They probably have not been stored by the solver because the option keep_details=True have not been set.
+            Please re-run the resolution with this option.""")
+
+        S, _ = self.green_function.evaluate(points, result.body.mesh, result.free_surface, result.water_depth, result.wavenumber)
+        potential = S @ result.sources  # Sum the contributions of all panels in the mesh
+        return potential.reshape(output_shape)
+
+
+    def compute_velocity(self, points, result):
+        """Compute the value of the velocity vector at given points for a previously solved potential flow problem.
+
+        Parameters
+        ----------
+        points: array of shape (3,) or (N, 3), or 3-ple of arrays returned by meshgrid, or cpt.Mesh or cpt.CollectionOfMeshes object
+            Coordinates of the point(s) at which the velocity should be computed
+        results: LinearPotentialFlowResult
+            The return of the BEM solver
+
+        Returns
+        -------
+        complex-valued array of shape (3,) or (N,, 3) or (nx, ny, nz, 3) or (mesh.nb_faces, 3) depending of the kind of input
+            The value of the velocity at the points
+
+        Raises
+        ------
+        Exception: if the :code:`LinearPotentialFlowResult` object given as input does not contain the source distribution.
+        """
+        points, output_shape = _normalize_points(points, keep_mesh=True)
+
+        if result.sources is None:
+            raise Exception(f"""The values of the sources of {result} cannot been found.
+            They probably have not been stored by the solver because the option keep_details=True have not been set.
+            Please re-run the resolution with this option.""")
+
+        _, gradG = self.green_function.evaluate(points, result.body.mesh, result.free_surface, result.water_depth, result.wavenumber,
+                                                early_dot_product=False)
+        velocities = np.einsum('ijk,j->ik', gradG, result.sources)  # Sum the contributions of all panels in the mesh
+        return velocities.reshape((*output_shape, 3))
+
+
+    def compute_pressure(self, points, result):
+        """Compute the value of the pressure at given points for a previously solved potential flow problem.
+
+        Parameters
+        ----------
+        points: array of shape (3,) or (N, 3), or 3-ple of arrays returned by meshgrid, or cpt.Mesh or cpt.CollectionOfMeshes object
+            Coordinates of the point(s) at which the pressure should be computed
+        results: LinearPotentialFlowResult
+            The return of the BEM solver
+
+        Returns
+        -------
+        complex-valued array of shape (1,) or (N,) or (nx, ny, nz) or (mesh.nb_faces,) depending of the kind of input
+            The value of the pressure at the points
+
+        Raises
+        ------
+        Exception: if the :code:`LinearPotentialFlowResult` object given as input does not contain the source distribution.
+        """
+        return 1j * result.omega * result.rho * self.compute_potential(points, results)
+
+
+    def compute_free_surface_elevation(self, points, result):
+        """Compute the value of the free surface elevation at given points for a previously solved potential flow problem.
+
+        Parameters
+        ----------
+        points: array of shape (2,) or (N, 2), or 2-ple of arrays returned by meshgrid, or cpt.Mesh or cpt.CollectionOfMeshes object
+            Coordinates of the point(s) at which the free surface elevation should be computed
+        results: LinearPotentialFlowResult
+            The return of the BEM solver
+
+        Returns
+        -------
+        complex-valued array of shape (1,) or (N,) or (nx, ny, nz) or (mesh.nb_faces,) depending of the kind of input
+            The value of the free surface elevation at the points
+
+        Raises
+        ------
+        Exception: if the :code:`LinearPotentialFlowResult` object given as input does not contain the source distribution.
+        """
+        points, output_shape = _normalize_free_surface_points(points, keep_mesh=True)
+
+        fs_elevation = 1j*result.omega/result.g * self.compute_potential(points, result)
+        return fs_elevation.reshape(output_shape)
+
+
+    ## Legacy
+
     def get_potential_on_mesh(self, result, mesh, chunk_size=50):
         """Compute the potential on a mesh for the potential field of a previously solved problem.
         Since the interaction matrix does not need to be computed in full to compute the matrix-vector product,
         only a few lines are evaluated at a time to reduce the memory cost of the operation.
 
+        The newer method :code:`compute_potential` should be prefered in the future.
+
         Parameters
         ----------
         result : LinearPotentialFlowResult
             the return of the BEM solver
         mesh : Mesh or CollectionOfMeshes
             a mesh
         chunk_size: int, optional
@@ -192,38 +310,40 @@
             They probably have not been stored by the solver because the option keep_details=True have not been set.
             Please re-run the resolution with this option.""")
 
         if chunk_size > mesh.nb_faces:
             S = self.engine.build_S_matrix(
                 mesh,
                 result.body.mesh,
-                result.free_surface, result.sea_bottom, result.wavenumber,
+                result.free_surface, result.water_depth, result.wavenumber,
                 self.green_function
             )
             phi = S @ result.sources
 
         else:
             phi = np.empty((mesh.nb_faces,), dtype=np.complex128)
             for i in range(0, mesh.nb_faces, chunk_size):
                 faces_to_extract = list(range(i, min(i+chunk_size, mesh.nb_faces)))
                 S = self.engine.build_S_matrix(
                     mesh.extract_faces(faces_to_extract),
                     result.body.mesh,
-                    result.free_surface, result.sea_bottom, result.wavenumber,
+                    result.free_surface, result.water_depth, result.wavenumber,
                     self.green_function
                 )
                 phi[i:i+chunk_size] = S @ result.sources
 
         LOG.debug(f"Done computing potential on {mesh.name} for {result}.")
 
         return phi
 
     def get_free_surface_elevation(self, result, free_surface, keep_details=False):
         """Compute the elevation of the free surface on a mesh for a previously solved problem.
 
+        The newer method :code:`compute_free_surface_elevation` should be prefered in the future.
+
         Parameters
         ----------
         result : LinearPotentialFlowResult
             the return of the solver
         free_surface : FreeSurface
             a meshed free surface
         keep_details : bool, optional
@@ -239,40 +359,7 @@
         Exception: if the :code:`Result` object given as input does not contain the source distribution.
         """
         fs_elevation = 1j*result.omega/result.g * self.get_potential_on_mesh(result, free_surface.mesh)
         if keep_details:
             result.fs_elevation[free_surface] = fs_elevation
         return fs_elevation
 
-
-# LEGACY INTERFACE
-
-def _arguments(f):
-    """Returns the name of the arguments of the function f"""
-    return f.__code__.co_varnames[:f.__code__.co_argcount]
-
-class Nemoh(BEMSolver):
-    """Solver for the BEM problem based on Nemoh's Green function. Legacy API.
-    Parameters are dispatched to the Delhommeau class and to the engine
-    (BasicMatrixEngine or HierarchicalToeplitzMatrixEngine).
-    """
-
-    def __init__(self, **params):
-        green_function = Delhommeau(
-           **{key: params[key] for key in params if key in _arguments(Delhommeau.__init__)}
-	)
-        if 'hierarchical_matrices' in params and params['hierarchical_matrices']:
-            engine = HierarchicalToeplitzMatrixEngine(
-               **{key: params[key] for key in params if key in _arguments(HierarchicalToeplitzMatrixEngine.__init__)}
-            )
-        else:
-            engine = BasicMatrixEngine(
-               **{key: params[key] for key in params if key in _arguments(BasicMatrixEngine.__init__)}
-            )
-
-        super().__init__(green_function=green_function, engine=engine)
-
-    def build_matrices(self, *args, **kwargs):
-        """Legacy API."""
-        args = args + (self.green_function,)
-        return self.engine.build_matrices(*args, **kwargs)
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `capytaine-1.5.post1/capytaine/bodies/bodies.py` & `capytaine-2.0/capytaine/bodies/bodies.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 import numpy as np
 import xarray as xr
 
 from capytaine.tools.optional_imports import silently_import_optional_dependency
 meshio = silently_import_optional_dependency("meshio")
 
-from capytaine.meshes.geometry import Abstract3DObject, Plane, inplace_transformation
+from capytaine.meshes.geometry import Abstract3DObject, ClippableMixin, Plane, inplace_transformation
 from capytaine.meshes.meshes import Mesh
 from capytaine.meshes.symmetric import build_regular_array_of_meshes
 from capytaine.meshes.collections import CollectionOfMeshes
 from capytaine.bodies.dofs import RigidBodyDofsPlaceholder
 
 LOG = logging.getLogger(__name__)
 
 TRANSLATION_DOFS_DIRECTIONS = {"surge": (1, 0, 0), "sway": (0, 1, 0), "heave": (0, 0, 1)}
 ROTATION_DOFS_AXIS = {"roll": (1, 0, 0), "pitch": (0, 1, 0), "yaw": (0, 0, 1)}
 
 
-class FloatingBody(Abstract3DObject):
+class FloatingBody(ClippableMixin, Abstract3DObject):
     """A floating body described as a mesh and some degrees of freedom.
 
     The mesh structure is stored as a Mesh from capytaine.mesh.mesh or a
     CollectionOfMeshes from capytaine.mesh.meshes_collection.
 
     The degrees of freedom (dofs) are stored as a dict associating a name to
     a complex-valued array of shape (nb_faces, 3). To each face of the body
@@ -75,28 +75,29 @@
             self.name = "dummy_body"
         elif name is None:
             self.name = self.mesh.name
         else:
             self.name = name
 
         self.mass = mass
-        self.center_of_mass = center_of_mass
+        if center_of_mass is not None:
+            self.center_of_mass = np.asarray(center_of_mass, dtype=float)
+        else:
+            self.center_of_mass = None
 
         if dofs is None:
             self.dofs = {}
         elif isinstance(dofs, RigidBodyDofsPlaceholder):
             if dofs.rotation_center is not None:
-                self.rotation_center = np.asarray(dofs.rotation_center)
+                self.rotation_center = np.asarray(dofs.rotation_center, dtype=float)
             self.dofs = {}
             self.add_all_rigid_body_dofs()
         else:
             self.dofs = dofs
 
-        self.full_body = None
-
         if self.mesh.nb_vertices == 0 or self.mesh.nb_faces == 0:
             LOG.warning(f"New floating body (with empty mesh!): {self.name}.")
         else:
             self.mesh.heal_mesh()
             LOG.info(f"New floating body: {self.name}.")
 
     @staticmethod
@@ -710,15 +711,17 @@
         hydrostatics["breadth_overall"] = full_breadth
         hydrostatics["depth"] = depth
         hydrostatics["draught"] = np.abs(coord_min[2])
         hydrostatics["length_at_waterline"] = wl_length
         hydrostatics["breadth_at_waterline"] = wl_breadth
         hydrostatics["length_overall_submerged"] = sub_length
         hydrostatics["breadth_overall_submerged"] = sub_breadth
-        self.inertia_matrix = hydrostatics["inertia_matrix"] = self.compute_rigid_body_inertia(rho=rho)
+        if any(dof.lower() in {"surge", "sway", "heave", "roll", "pitch", "yaw"}
+               for dof in self.dofs) > 0: # If there is at least one rigid body dof:
+            self.inertia_matrix = hydrostatics["inertia_matrix"] = self.compute_rigid_body_inertia(rho=rho)
 
         return hydrostatics
 
 
     ###################
     # Transformations #
     ###################
@@ -734,15 +737,15 @@
 
         if all(body.mass is not None for body in bodies):
             new_mass = sum(body.mass for body in bodies)
         else:
             new_mass = None
 
         if (all(body.mass is not None for body in bodies)
-                and all(body.center_of_mass for body in bodies)):
+                and all(body.center_of_mass is not None for body in bodies)):
             new_cog = sum(body.mass*np.asarray(body.center_of_mass) for body in bodies)/new_mass
         else:
             new_cog = None
 
         joined_bodies = FloatingBody(
             mesh=meshes, dofs=dofs, mass=new_mass, center_of_mass=new_cog, name=name
             )
@@ -922,76 +925,61 @@
             self.dofs[dof] -= 2 * np.outer(np.dot(self.dofs[dof], plane.normal), plane.normal)
         for point_attr in ('geometric_center', 'rotation_center', 'center_of_mass'):
             if point_attr in self.__dict__ and self.__dict__[point_attr] is not None:
                 self.__dict__[point_attr] -= 2 * (np.dot(self.__dict__[point_attr], plane.normal) - plane.c) * plane.normal
         return self
 
     @inplace_transformation
-    def translate(self, *args):
-        self.mesh.translate(*args)
+    def translate(self, vector, *args, **kwargs):
+        self.mesh.translate(vector, *args, **kwargs)
         for point_attr in ('geometric_center', 'rotation_center', 'center_of_mass'):
             if point_attr in self.__dict__ and self.__dict__[point_attr] is not None:
-                self.__dict__[point_attr] += args[0]
+                self.__dict__[point_attr] += vector
         return self
 
     @inplace_transformation
     def rotate(self, axis, angle):
         self.mesh.rotate(axis, angle)
         for point_attr in ('geometric_center', 'rotation_center', 'center_of_mass'):
             if point_attr in self.__dict__ and self.__dict__[point_attr] is not None:
                 self.__dict__[point_attr] = axis.rotate_points([self.__dict__[point_attr]], angle)
         for dof in self.dofs:
             self.dofs[dof] = axis.rotate_vectors(self.dofs[dof], angle)
         return self
 
     @inplace_transformation
     def clip(self, plane):
-        # Keep of copy of the full mesh
-        if self.full_body is None:
-            self.full_body = self.copy()
-
         # Clip mesh
         LOG.info(f"Clipping {self.name} with respect to {plane}")
         self.mesh.clip(plane)
 
         # Clip dofs
         ids = self.mesh._clipping_data['faces_ids']
         for dof in self.dofs:
             if len(ids) > 0:
                 self.dofs[dof] = np.array(self.dofs[dof])[ids]
             else:
                 self.dofs[dof] = np.empty((0, 3))
         return self
 
-    def clipped(self, plane, **kwargs):
-        # Same API as for the other transformations
-        return self.clip(plane, inplace=False, **kwargs)
-
-    @inplace_transformation
-    def keep_immersed_part(self, free_surface=0.0, sea_bottom=-np.infty):
-        """Remove the parts of the mesh above the sea bottom and below the free surface."""
-        self.clip(Plane(normal=(0, 0, 1), point=(0, 0, free_surface)))
-        if sea_bottom > -np.infty:
-            self.clip(Plane(normal=(0, 0, -1), point=(0, 0, sea_bottom)))
-        return self
-
-    def immersed_part(self, free_surface=0.0, sea_bottom=-np.infty):
-        return self.keep_immersed_part(free_surface, sea_bottom, inplace=False, name=self.name)
 
     #############
     #  Display  #
     #############
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return (f"{self.__class__.__name__}(mesh={self.mesh.name}, "
                 f"dofs={{{', '.join(self.dofs.keys())}}}, name={self.name})")
 
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__repr__())
+
     def show(self, **kwargs):
         from capytaine.ui.vtk.body_viewer import FloatingBodyViewer
         viewer = FloatingBodyViewer()
         viewer.add_body(self, **kwargs)
         viewer.show()
         viewer.finalize()
 
@@ -1018,7 +1006,12 @@
             missing_dofs = set(motion.keys()) - set(self.dofs.keys())
             raise ValueError(f"Trying to animate the body {self.name} using dof(s) {missing_dofs}, but no dof of this name is defined for {self.name}.")
 
         animation = Animation(*args, **kwargs)
         animation._add_actor(self.mesh.merged(), faces_motion=sum(motion[dof_name] * dof for dof_name, dof in self.dofs.items() if dof_name in motion))
         return animation
 
+    @property
+    def minimal_computable_wavelength(self):
+        """For accuracy of the resolution, wavelength should not be smaller than this value."""
+        return 8*self.mesh.faces_radiuses.max()
+
```

### Comparing `capytaine-1.5.post1/capytaine/bodies/predefined/cylinders.py` & `capytaine-2.0/capytaine/bodies/predefined/cylinders.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/bodies/predefined/rectangles.py` & `capytaine-2.0/capytaine/bodies/predefined/rectangles.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/bodies/predefined/spheres.py` & `capytaine-2.0/capytaine/bodies/predefined/spheres.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/green_functions/delhommeau.py` & `capytaine-2.0/capytaine/green_functions/delhommeau.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 import logging
 from functools import lru_cache
 from importlib import import_module
 
 import numpy as np
 
+from capytaine.meshes.meshes import Mesh
+from capytaine.meshes.collections import CollectionOfMeshes
 from capytaine.tools.prony_decomposition import exponential_decomposition, error_exponential_decomposition
 
 from capytaine.green_functions.abstract_green_function import AbstractGreenFunction
 
 LOG = logging.getLogger(__name__)
 
 
@@ -30,15 +32,15 @@
         Number of tabulation points for vertical distance.
         If 0 is given, the no tabulation is used.
         Default: 46, as in Nemoh.
     tabulation_nb_integration_points: int, optional
         Number of points for the numerical integration w.r.t. :math:`theta` of Delhommeau's integrals
         Default: 251, as in Nemoh.
     finite_depth_prony_decomposition_method: string, optional
-        The implementation of the Prony decomposition used to compute the finite depth Green function.
+        The implementation of the Prony decomposition used to compute the finite water_depth Green function.
         Accepted values: :code:`'fortran'` for Nemoh's implementation (by default), :code:`'python'` for an experimental Python implementation.
         See :func:`find_best_exponential_decomposition`.
     floating_point_precision: string, optional
         Either :code:`'float32'` for single precision computations or :code:`'float64'` for double precision computations.
         Default: :code:`'float64'`.
 
     Attributes
@@ -49,16 +51,16 @@
     tabulated_integrals: numpy.array of shape (tabulation_nr, tabulation_nz, 2, 2) and type floating_point_precision
         Tabulated Delhommeau integrals.
     """
 
     fortran_core_basename = "Delhommeau"
 
     def __init__(self, *,
-                 tabulation_nr=328,
-                 tabulation_nz=46,
+                 tabulation_nr=400,
+                 tabulation_nz=80,
                  tabulation_nb_integration_points=251,
                  finite_depth_prony_decomposition_method='fortran',
                  floating_point_precision='float64',
                  ):
 
         self.fortran_core = import_module(f"capytaine.green_functions.libs.{self.fortran_core_basename}_{floating_point_precision}")
 
@@ -80,17 +82,30 @@
         }
 
         self._hash = hash(self.exportable_settings.values())
 
     def __hash__(self):
         return self._hash
 
+    def __str__(self):
+        params = f"tabulation_nz={self.exportable_settings['tabulation_nz']}"
+        params += f", tabulation_nr={self.exportable_settings['tabulation_nr']}"
+        params += f", tabulation_nb_integration_points={self.exportable_settings['tabulation_nb_integration_points']}"
+        params += f", floating_point_precision=\'{self.exportable_settings['floating_point_precision']}\'"
+        return f"{self.__class__.__name__}({params})"
+
+    def __repr__(self):
+        return self.__str__()
+
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__str__())
+
     @lru_cache(maxsize=128)
     def find_best_exponential_decomposition(self, dimensionless_omega, dimensionless_wavenumber):
-        """Compute the decomposition of a part of the finite depth Green function as a sum of exponential functions.
+        """Compute the decomposition of a part of the finite water_depth Green function as a sum of exponential functions.
 
         Two implementations are available: the legacy Fortran implementation from Nemoh and a newer one written in Python.
         For some still unexplained reasons, the two implementations do not always give the exact same result.
         Until the problem is better understood, the Fortran implementation is the default one, to ensure consistency with Nemoh.
         The Fortran version is also significantly faster...
 
         Results are cached.
@@ -106,15 +121,15 @@
 
         Returns
         -------
         Tuple[np.ndarray, np.ndarray]
             the amplitude and growth rates of the exponentials
         """
 
-        LOG.debug(f"\tCompute Prony decomposition in finite depth Green function "
+        LOG.debug(f"\tCompute Prony decomposition in finite water_depth Green function "
                   f"for dimless_omega=%.2e and dimless_wavenumber=%.2e",
                   dimensionless_omega, dimensionless_wavenumber)
 
         if self.finite_depth_prony_decomposition_method.lower() == 'python':
             # The function that will be approximated.
             @np.vectorize
             def f(x):
@@ -148,84 +163,104 @@
         # Add one more exponential function (actually a constant).
         # It is not clear where it comes from exactly in the theory...
         a = np.concatenate([a, np.array([2])])
         lamda = np.concatenate([lamda, np.array([0.0])])
 
         return a, lamda
 
-    def evaluate(self, mesh1, mesh2, free_surface=0.0, sea_bottom=-np.infty, wavenumber=1.0):
+    def evaluate(self, mesh1, mesh2, free_surface=0.0, water_depth=np.infty, wavenumber=1.0, early_dot_product=True):
         r"""The main method of the class, called by the engine to assemble the influence matrices.
 
         Parameters
         ----------
-        mesh1: Mesh or CollectionOfMeshes
+        mesh1: Mesh or CollectionOfMeshes or list of points
             mesh of the receiving body (where the potential is measured)
+            if only S is wanted or early_dot_product is False, then only a list of points as an array of shape (n, 3) can be passed.
         mesh2: Mesh or CollectionOfMeshes
             mesh of the source body (over which the source distribution is integrated)
         free_surface: float, optional
             position of the free surface (default: :math:`z = 0`)
-        sea_bottom: float, optional
-            position of the sea bottom (default: :math:`z = -\infty`)
+        water_depth: float, optional
+            constant depth of water (default: :math:`+\infty`)
         wavenumber: float, optional
             wavenumber (default: 1.0)
+        early_dot_product: boolean, optional
+            if False, return K as a (n, m, 3) array storing ∫∇G
+            if True, return K as a (n, m) array storing ∫∇G·n
 
         Returns
         -------
         tuple of numpy arrays
             the matrices :math:`S` and :math:`K`
         """
 
-        depth = free_surface - sea_bottom
         if free_surface == np.infty: # No free surface, only a single Rankine source term
 
             a_exp, lamda_exp = np.empty(1), np.empty(1)  # Dummy arrays that won't actually be used by the fortran code.
 
             coeffs = np.array((1.0, 0.0, 0.0))
 
-        elif depth == np.infty:
+        elif water_depth == np.infty:
 
             a_exp, lamda_exp = np.empty(1), np.empty(1)  # Idem
 
             if wavenumber == 0.0:
                 coeffs = np.array((1.0, 1.0, 0.0))
             elif wavenumber == np.infty:
                 coeffs = np.array((1.0, -1.0, 0.0))
             else:
                 coeffs = np.array((1.0, 1.0, 1.0))
 
-        else:  # Finite depth
+        else:  # Finite water_depth
             a_exp, lamda_exp = self.find_best_exponential_decomposition(
-                wavenumber*depth*np.tanh(wavenumber*depth),
-                wavenumber*depth,
+                wavenumber*water_depth*np.tanh(wavenumber*water_depth),
+                wavenumber*water_depth,
             )
             if wavenumber == 0.0:
                 raise NotImplementedError
             elif wavenumber == np.infty:
                 raise NotImplementedError
             else:
                 coeffs = np.array((1.0, 1.0, 1.0))
 
+        if isinstance(mesh1, Mesh) or isinstance(mesh1, CollectionOfMeshes):
+            collocation_points = mesh1.faces_centers
+            nb_collocation_points = mesh1.nb_faces
+            early_dot_product_normals = mesh1.faces_normals
+        elif isinstance(mesh1, np.ndarray) and mesh1.ndim ==2 and mesh1.shape[1] == 3:
+            collocation_points = mesh1
+            nb_collocation_points = mesh1.shape[0]
+            early_dot_product_normals = np.zeros((nb_collocation_points, 3))  # Hopefully unused
+        else:
+            raise ValueError(f"Unrecognized input for {self.__class__.__name__}.evaluate")
+
+        S = np.empty((nb_collocation_points, mesh2.nb_faces), order="F", dtype="complex128")
+        K = np.empty((nb_collocation_points, mesh2.nb_faces, 1 if early_dot_product else 3), order="F", dtype="complex128")
+
         # Main call to Fortran code
-        S, K = self.fortran_core.matrices.build_matrices(
-            mesh1.faces_centers, mesh1.faces_normals,
+        self.fortran_core.matrices.build_matrices(
+            collocation_points,  early_dot_product_normals,
             mesh2.vertices,      mesh2.faces + 1,
             mesh2.faces_centers, mesh2.faces_normals,
             mesh2.faces_areas,   mesh2.faces_radiuses,
             *mesh2.quadrature_points,
-            wavenumber, depth,
+            wavenumber, water_depth,
             coeffs,
             self.tabulated_r_range, self.tabulated_z_range, self.tabulated_integrals,
             lamda_exp, a_exp,
-            mesh1 is mesh2
+            mesh1 is mesh2,
+            S, K
         )
 
         if np.any(np.isnan(S)) or np.any(np.isnan(K)):
             raise RuntimeError("Green function returned a NaN in the interaction matrix.\n"
                     "It could be due to overlapping panels.")
 
+        if early_dot_product: K = K.reshape((nb_collocation_points, mesh2.nb_faces))
+
         return S, K
 
 ################################
 
 class XieDelhommeau(Delhommeau):
     """Variant of Nemoh's Green function, more accurate near the free surface.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/Delhommeau_integrals.f90` & `capytaine-2.0/capytaine/green_functions/libDelhommeau/src/Delhommeau_integrals.f90`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/Green_Rankine.f90` & `capytaine-2.0/capytaine/green_functions/libDelhommeau/src/Green_Rankine.f90`

 * *Files 8% similar despite different names*

```diff
@@ -122,21 +122,23 @@
 
     ! Outputs
     REAL(KIND=PRE),               INTENT(OUT) :: S0
     REAL(KIND=PRE), DIMENSION(3), INTENT(OUT) :: VS0
 
     ! Local variables
     REAL(KIND=PRE) :: RO
-
-    RO = NORM2(M(1:3) - Face_center(1:3)) ! Distance from center of mass of the face to M.
+    REAL(KIND=PRE), DIMENSION(3) :: VO
+    
+    VO = Face_center - M
+    RO = NORM2(VO) ! Distance from center of mass of the face to M.
 
     IF (RO > REAL(1e-7, KIND=PRE)) THEN
       ! Asymptotic value if face far away from M
       S0       = Face_area/RO
-      VS0(1:3) = (Face_center(1:3) - M)*S0/RO**2
+      VS0(1:3) = VO*S0/RO**2
     ELSE
       ! Singularity...
       S0 = ZERO
       VS0(1:3) = ZERO
     END IF
 
   END SUBROUTINE COMPUTE_ASYMPTOTIC_RANKINE_SOURCE
```

### Comparing `capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/Green_wave.f90` & `capytaine-2.0/capytaine/green_functions/libDelhommeau/src/Green_wave.f90`

 * *Files 3% similar despite different names*

```diff
@@ -41,64 +41,63 @@
     REAL(KIND=PRE), DIMENSION(size(tabulated_r_range), size(tabulated_z_range), 2, 2), INTENT(IN) :: tabulated_integrals
 
     ! Outputs
     COMPLEX(KIND=PRE),                        INTENT(OUT) :: FS  ! the integral
     COMPLEX(KIND=PRE), DIMENSION(3),          INTENT(OUT) :: VS  ! its gradient
 
     ! Local variables
-    REAL(KIND=PRE) :: r, z, r1, drdx, drdy
+    REAL(KIND=PRE) :: r, z, r1, drdx1, drdx2, dzdx3
     REAL(KIND=PRE), dimension(2, 2) :: integrals
 
     r = wavenumber * NORM2(X0I(1:2) - X0J(1:2))
     z = wavenumber * (X0I(3) + X0J(3))
     r1 = hypot(r, z)
 
     IF (ABS(r) > 16*EPSILON(r)) THEN
-      drdx = wavenumber * (X0I(1) - X0J(1))/r
-      drdy = wavenumber * (X0I(2) - X0J(2))/r
+      drdx1 = wavenumber**2 * (X0I(1) - X0J(1))/r
+      drdx2 = wavenumber**2 * (X0I(2) - X0J(2))/r
     ELSE
       ! Limit when r->0 is not well defined...
-      drdx = ZERO
-      drdy = ZERO
+      drdx1 = ZERO
+      drdx2 = ZERO
     END IF
+    dzdx3 = wavenumber
 
     IF (z > -1e-8) THEN
       PRINT*, "Error: Impossible to compute the wave part of the Green function due to panels on the free surface (z=0) or above."
       ERROR STOP
     ENDIF
 
     !=======================================================
     ! Evaluate the elementary integrals depending on z and r
     !=======================================================
     IF ((size(tabulated_z_range) <= 1) .or. (size(tabulated_r_range) <= 1)) THEN
       ! No tabulation, fully recompute the Green function each time.
       integrals = numerical_integration(r, z, 500)
-
     ELSE
-      IF ((MINVAL(tabulated_z_range) < z) .AND. (r < MAXVAL(tabulated_r_range))) THEN
+      IF ((abs(z) < abs(tabulated_z_range(size(tabulated_z_range)))) .AND. (r < tabulated_r_range(size(tabulated_r_range)))) THEN
         ! Within the range of tabulated data
         integrals = pick_in_default_tabulation(r, z, tabulated_r_range, tabulated_z_range, tabulated_integrals)
-
       ELSE
         ! Asymptotic expression for distant panels
         integrals = asymptotic_approximations(MAX(r, 1e-10), z)
       ENDIF
     ENDIF
 
     !================================================
     ! Add the elementary integrals to build FS and VS
     !================================================
 
     FS    = CMPLX(integrals(1, 2), integrals(2, 2), KIND=PRE)
-    VS(1) = -drdx * CMPLX(integrals(1, 1), integrals(2, 1), KIND=PRE)
-    VS(2) = -drdy * CMPLX(integrals(1, 1), integrals(2, 1), KIND=PRE)
+    VS(1) = -drdx1 * CMPLX(integrals(1, 1), integrals(2, 1), KIND=PRE)
+    VS(2) = -drdx2 * CMPLX(integrals(1, 1), integrals(2, 1), KIND=PRE)
 #ifdef XIE_CORRECTION
-    VS(3) = CMPLX(integrals(1, 2) + ONE/r1, integrals(2, 2), KIND=PRE)
+    VS(3) = dzdx3 * CMPLX(integrals(1, 2) + ONE/r1, integrals(2, 2), KIND=PRE)
 #else
-    VS(3) = CMPLX(integrals(1, 2), integrals(2, 2), KIND=PRE)
+    VS(3) = dzdx3 * CMPLX(integrals(1, 2), integrals(2, 2), KIND=PRE)
 #endif
 
     RETURN
   END SUBROUTINE COLLECT_DELHOMMEAU_INTEGRALS
 
   ! =========================
 
@@ -128,15 +127,15 @@
 
     ! The integrals
     CALL COLLECT_DELHOMMEAU_INTEGRALS(                           &
       X0I, X0J, wavenumber,                                      &
       tabulated_r_range, tabulated_z_range, tabulated_integrals, &
       SP, VSP(:))
     SP  = 2*wavenumber*SP
-    VSP = 2*wavenumber**2*VSP
+    VSP = 2*wavenumber*VSP
 
 #ifndef XIE_CORRECTION
     ! In the original Delhommeau method
     XJ_REFLECTION(1:2) = X0J(1:2)
     XJ_REFLECTION(3) = - X0J(3)
     ! Only one singularity is missing in the derivative
     VSP = VSP - 2*(X0I - XJ_REFLECTION)/(NORM2(X0I-XJ_REFLECTION)**3)
@@ -257,16 +256,16 @@
 
     ! Multiply by some coefficients
     AMH  = wavenumber*depth
     AKH  = AMH*TANH(AMH)
     A    = (AMH+AKH)**2/(2*depth*(AMH**2-AKH**2+AKH))
 
     SP          = A*SP
-    VSP_ANTISYM = A*wavenumber*VSP_ANTISYM
-    VSP_SYM     = A*wavenumber*VSP_SYM
+    VSP_ANTISYM = A*VSP_ANTISYM
+    VSP_SYM     = A*VSP_SYM
 
     !=====================================================
     ! Part 2: Integrate (NEXP+1)×4 terms of the form 1/MM'
     !=====================================================
 
     DO KE = 1, NEXP
       XI(:) = X0I(:)
```

### Comparing `capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/matrices.f90` & `capytaine-2.0/capytaine/green_functions/libDelhommeau/src/matrices.f90`

 * *Files 14% similar despite different names*

```diff
@@ -56,20 +56,20 @@
     REAL(KIND=PRE), DIMENSION(:, :, :, :),    INTENT(IN) :: tabulated_integrals
 
     ! Prony decomposition for finite depth
     INTEGER,                                  INTENT(IN) :: NEXP
     REAL(KIND=PRE), DIMENSION(NEXP),          INTENT(IN) :: AMBDA, AR
 
     ! Output
-    COMPLEX(KIND=PRE), DIMENSION(nb_faces_1, nb_faces_2), INTENT(OUT) :: S
-    COMPLEX(KIND=PRE), DIMENSION(nb_faces_1, nb_faces_2), INTENT(OUT) :: K
+    COMPLEX(KIND=PRE), DIMENSION(:, :), INTENT(INOUT) :: S
+    COMPLEX(KIND=PRE), DIMENSION(:, :, :), INTENT(INOUT) :: K
 
     ! Local variables
     INTEGER                         :: I, J, Q
-    REAL(KIND=PRE), DIMENSION(3)    :: reflected_centers_1_I, reflected_normals_1_I
+    REAL(KIND=PRE), DIMENSION(3)    :: reflected_centers_1_I, reflected_VSP1
     REAL(KIND=PRE)                  :: SP1
     REAL(KIND=PRE), DIMENSION(3)    :: VSP1
     COMPLEX(KIND=PRE)               :: SP2
     COMPLEX(KIND=PRE), DIMENSION(3) :: VSP2_SYM, VSP2_ANTISYM
     LOGICAL :: use_symmetry_of_wave_part
 
     use_symmetry_of_wave_part = ((SAME_BODY) .AND. (nb_quad_points == 1))
@@ -84,22 +84,22 @@
     ENDIF
 #endif
 
     coeffs(:) = coeffs(:)/(4*PI)
 
 
     !$OMP PARALLEL DO SCHEDULE(DYNAMIC) &
-    !$OMP&  PRIVATE(J, I, SP1, VSP1, SP2, VSP2_SYM, VSP2_ANTISYM, reflected_centers_1_I, reflected_normals_1_I)
+    !$OMP&  PRIVATE(J, I, SP1, VSP1, SP2, VSP2_SYM, VSP2_ANTISYM, reflected_centers_1_I, reflected_VSP1)
     DO J = 1, nb_faces_2
 
       !!!!!!!!!!!!!!!!!!!!
       !  Initialization  !
       !!!!!!!!!!!!!!!!!!!!
       S(:, J) = CMPLX(0.0, 0.0, KIND=PRE)
-      K(:, J) = CMPLX(0.0, 0.0, KIND=PRE)
+      K(:, J, :) = CMPLX(0.0, 0.0, KIND=PRE)
 
       !!!!!!!!!!!!!!!!!!
       !  Rankine part  !
       !!!!!!!!!!!!!!!!!!
       IF (coeffs(1) .NE. ZERO) THEN
         DO I = 1, nb_faces_1
 
@@ -111,15 +111,19 @@
             areas_2(J),                            &
             radiuses_2(J),                         &
             SP1, VSP1                              &
             )
 
           ! Store into influence matrix
           S(I, J) = S(I, J) - coeffs(1) * SP1                                ! Green function
-          K(I, J) = K(I, J) - coeffs(1) * DOT_PRODUCT(normals_1(I, :), VSP1) ! Gradient of the Green function
+          if (size(K, 3) == 1) then
+            K(I, J, 1) = K(I, J, 1) - coeffs(1) * DOT_PRODUCT(normals_1(I, :), VSP1(:))
+          else
+            K(I, J, :) = K(I, J, :) - coeffs(1) * VSP1(:)
+          endif
 
         END DO
       END IF
 
 
       !!!!!!!!!!!!!!!!!!!!!!!!!!!!
       !  Reflected Rankine part  !
@@ -134,30 +138,34 @@
             reflected_centers_1_I(3)   = -centers_1(I, 3)
           ELSE
             ! Reflection through sea bottom
             reflected_centers_1_I(1:2) = centers_1(I, 1:2)
             reflected_centers_1_I(3)   = -centers_1(I, 3) - 2*depth
           END IF
 
-          reflected_normals_1_I(1:2) = normals_1(I, 1:2)
-          reflected_normals_1_I(3)   = -normals_1(I, 3)
-
           CALL COMPUTE_INTEGRAL_OF_RANKINE_SOURCE( &
             reflected_centers_1_I(:),                &
             vertices_2(faces_2(J, :), :),          &
             centers_2(J, :),                       &
             normals_2(J, :),                       &
             areas_2(J),                            &
             radiuses_2(J),                         &
             SP1, VSP1                              &
             )
 
+          reflected_VSP1(1:2) = VSP1(1:2)
+          reflected_VSP1(3) = -VSP1(3)
+
           ! Store into influence matrix
           S(I, J) = S(I, J) - coeffs(2) * SP1                                ! Green function
-          K(I, J) = K(I, J) - coeffs(2) * DOT_PRODUCT(reflected_normals_1_I(:), VSP1) ! Gradient of the Green function
+          if (size(K, 3) == 1) then
+            K(I, J, 1) = K(I, J, 1) - coeffs(2) * DOT_PRODUCT(normals_1(I, :), reflected_VSP1(:))
+          else
+            K(I, J, :) = K(I, J, :) - coeffs(2) * reflected_VSP1(:)
+          endif
         END DO
       END IF
 
       !!!!!!!!!!!!!!!
       !  Wave part  !
       !!!!!!!!!!!!!!!
 
@@ -182,23 +190,32 @@
                 tabulated_r_range, tabulated_z_range, tabulated_integrals, &
                 NEXP, AMBDA, AR,            &
                 SP2, VSP2_SYM, VSP2_ANTISYM &
                 )
             END IF
 
             S(I, J) = S(I, J) - coeffs(3) * SP2 * quad_weights(J, Q)
-            K(I, J) = K(I, J) - coeffs(3) * &
-              DOT_PRODUCT(normals_1(I, :), VSP2_SYM + VSP2_ANTISYM) * quad_weights(J, Q)
+
+            if (size(K, 3) == 1) then
+              K(I, J, 1) = K(I, J, 1) - coeffs(3) * &
+                DOT_PRODUCT(normals_1(I, :), VSP2_SYM + VSP2_ANTISYM) * quad_weights(J, Q)
+            else
+              K(I, J, :) = K(I, J, :) - coeffs(3) * (VSP2_SYM + VSP2_ANTISYM) * quad_weights(J, Q)
+            endif
 
           END DO
         END DO
       END IF
 
       IF (SAME_BODY) THEN
-        K(J, J) = K(J, J) + 0.5
+        if (size(K, 3) == 1) then
+          K(J, J, 1) = K(J, J, 1) + 0.5
+        else
+          K(J, J, :) = K(J, J, :) + 0.5 * normals_1(J, :)
+        endif
       END IF
 
     END DO  ! parallelized loop on J
 
 
     IF ((coeffs(3) .NE. ZERO) .AND. use_symmetry_of_wave_part) THEN
       ! If we are computing the influence of some cells upon themselves, the resulting matrices have some symmetries.
@@ -227,22 +244,30 @@
               tabulated_r_range, tabulated_z_range, tabulated_integrals, &
               NEXP, AMBDA, AR,            &
               SP2, VSP2_SYM, VSP2_ANTISYM &
               )
           END IF
 
           S(I, J) = S(I, J) - coeffs(3) * SP2 * quad_weights(J, 1)
-          K(I, J) = K(I, J) - coeffs(3) * &
-            DOT_PRODUCT(normals_1(I, :), VSP2_SYM + VSP2_ANTISYM) * quad_weights(J, 1)
+          if (size(K, 3) == 1) then
+            K(I, J, 1) = K(I, J, 1) - coeffs(3) * &
+              DOT_PRODUCT(normals_1(I, :), VSP2_SYM + VSP2_ANTISYM) * quad_weights(J, 1)
+          else
+            K(I, J, :) = K(I, J, :) - coeffs(3) * (VSP2_SYM + VSP2_ANTISYM) * quad_weights(J, 1)
+          endif
 
           IF (.NOT. I==J) THEN
             VSP2_SYM(1:2) = -VSP2_SYM(1:2)
             S(J, I) = S(J, I) - coeffs(3) * SP2 * quad_weights(I, 1)
-            K(J, I) = K(J, I) - coeffs(3) * &
-              DOT_PRODUCT(normals_1(J, :), VSP2_SYM - VSP2_ANTISYM) * quad_weights(I, 1)
+            if (size(K, 3) == 1) then
+              K(J, I, 1) = K(J, I, 1) - coeffs(3) * &
+                DOT_PRODUCT(normals_1(J, :), VSP2_SYM - VSP2_ANTISYM) * quad_weights(I, 1)
+            else
+              K(J, I, :) = K(J, I, :) - coeffs(3) * (VSP2_SYM - VSP2_ANTISYM) * quad_weights(I, 1)
+            endif
           END IF
         END DO
       END DO
     END IF
 
   END SUBROUTINE
```

### Comparing `capytaine-1.5.post1/capytaine/green_functions/libDelhommeau/src/old_Prony_decomposition.f90` & `capytaine-2.0/capytaine/green_functions/libDelhommeau/src/old_Prony_decomposition.f90`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/io/bemio.py` & `capytaine-2.0/capytaine/io/bemio.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
                 temp_dict = {}
                 temp_dict['body_name'] = bemio_obj.body[i].name
                 temp_dict['water_depth'] = bemio_obj.body[i].water_depth
                 temp_dict['omega'] = omega
                 temp_dict['rho'] = rho
                 temp_dict['g'] = g
                 temp_dict['wave_direction'] = np.radians(dir)
-                temp_dict['convention'] = bemio_obj.body[i].bem_code
                 temp_dict['influenced_dof'] = dofs
                 
                 if wavenumber or wavelength:
                     if temp_dict['water_depth'] == np.infty or omega**2*temp_dict['water_depth']/temp_dict['g'] > 20:
                         k = omega**2/temp_dict['g']
                     else:
                         k = newton(lambda x: x*np.tanh(x) - omega**2*temp_dict['water_depth']/temp_dict['g'], x0=1.0)/temp_dict['water_depth']
@@ -134,8 +133,8 @@
 
                 rad_dict.append(temp_dict)
 
     df = df.append(pd.DataFrame.from_dict(difr_dict).explode(['influenced_dof', 'diffraction_force', 'Froude_Krylov_force']))
     df = df.append(pd.DataFrame.from_dict(rad_dict).explode(['influenced_dof', 'added_mass', 'radiation_damping']))
     df = df.astype({'added_mass': np.float64, 'radiation_damping': np.float64, 'diffraction_force': np.complex128, 'Froude_Krylov_force': np.complex128})
 
-    return df
+    return df
```

### Comparing `capytaine-1.5.post1/capytaine/io/legacy.py` & `capytaine-2.0/capytaine/io/legacy.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,17 @@
     """Read a Nemoh.cal file and return a list of problems."""
 
     with open(filepath, 'r') as cal_file:
 
         cal_file.readline()  # Unused line.
         rho = float(cal_file.readline().split()[0])
         g = float(cal_file.readline().split()[0])
-        depth = float(cal_file.readline().split()[0])
-        if depth == 0.0:
-            sea_bottom = -np.infty
-        else:
-            sea_bottom = -depth
+        water_depth = float(cal_file.readline().split()[0])
+        if water_depth == 0.0:
+            water_depth = np.infty
         xeff, yeff = (float(x) for x in cal_file.readline().split()[0:2])
 
         bodies = []
 
         cal_file.readline()  # Unused line.
         nb_bodies = int(cal_file.readline().split()[0])
         for _ in range(nb_bodies):
@@ -80,16 +78,29 @@
 
         if nb_bodies > 1:
             bodies = FloatingBody.join_bodies(*bodies)
         else:
             bodies = bodies[0]
 
         cal_file.readline()  # Unused line.
-        frequency_data = cal_file.readline().split()
-        omega_range = np.linspace(float(frequency_data[1]), float(frequency_data[2]), int(frequency_data[0]))
+        frequency_data_string_without_comment = cal_file.readline().split('!')[0]
+        frequency_data = frequency_data_string_without_comment.split()
+        if len(frequency_data) == 3:  # Nemoh v2 format
+            omega_range = np.linspace(float(frequency_data[1]), float(frequency_data[2]), int(frequency_data[0]))
+        else:
+            type_of_frequency_data = int(frequency_data[0])
+            if type_of_frequency_data == 1:  # angular frequency
+                omega_range = np.linspace(float(frequency_data[2]), float(frequency_data[3]), int(frequency_data[1]))
+            elif type_of_frequency_data == 2:  # frequency
+                omega_range = 2*np.pi*np.linspace(float(frequency_data[2]), float(frequency_data[3]), int(frequency_data[1]))
+            elif type_of_frequency_data == 3:  # period
+                omega_range = 2*np.pi/np.linspace(float(frequency_data[2]), float(frequency_data[3]), int(frequency_data[1]))
+            else:
+                raise ValueError(f"Cannot parse the frequency data \"{frequency_data_string_without_comment}\" in {filepath}.")
+
 
         direction_data = cal_file.readline().split()
         direction_range = np.linspace(float(direction_data[1]), float(direction_data[2]), int(direction_data[0]))
         direction_range = np.pi/180*direction_range  # conversion from degrees to radians.
 
         # The options below are not implemented yet.
 
@@ -97,15 +108,15 @@
         irf_data = cal_file.readline()
         show_pressure = cal_file.readline().split()[0] == "1"
         kochin_data = cal_file.readline().split()
         kochin_range = np.linspace(float(kochin_data[1]), float(kochin_data[2]), int(kochin_data[0]))
         free_surface_data = cal_file.readline().split()
 
     # Generate Capytaine's problem objects
-    env_args = dict(body=bodies, rho=rho, sea_bottom=sea_bottom, g=g)
+    env_args = dict(body=bodies, rho=rho, water_depth=water_depth, g=g)
     problems = []
     for omega in omega_range:
         for direction in direction_range:
             problems.append(DiffractionProblem(wave_direction=direction, omega=omega, **env_args))
         for dof in bodies.dofs:
             problems.append(RadiationProblem(radiating_dof=dof, omega=omega, **env_args))
 
@@ -154,15 +165,15 @@
 
     # Write Nemoh.cal
     with open(os.path.join(directory_name, "Nemoh.cal"), "w") as nemoh_cal:
         nemoh_cal.write(
                 DEFAULT_NEMOH_CAL.format(
                     rho=problem.rho,
                     g=problem.g,
-                    depth=problem.depth if problem.depth < np.infty else 0,
+                    depth=problem.water_depth if problem.water_depth < np.infty else 0,
                     mesh_filename=f'{problem.body.name}.dat',
                     mesh_vertices=problem.body.mesh.nb_vertices,
                     mesh_faces=problem.body.mesh.nb_faces,
                     omega_nb_steps=omega_nb_steps,
                     omega_start=omega_start,
                     omega_stop=omega_stop,
                     )
@@ -242,7 +253,44 @@
                         val = data['excitation_force'].sel(omega=o, wave_direction=wave_direction, influenced_dof=dof).values
                         fi.write(f'{np.abs(val):e}')
                         fi.write('  ')
                         fi.write(f'{np.angle(val):e}')
                         fi.write('  ')
                     fi.write('\n')
 
+def export_hydrostatics(hydrostatics_directory, bodies):
+    """Determine filenames (following Nemoh convention) and call the .dat file writer"""
+
+    if os.path.isdir(hydrostatics_directory):
+        LOG.warning(f"""Exporting problem in already existing directory: {hydrostatics_directory}
+             You might be overwriting existing files!""")
+    else:
+        os.makedirs(hydrostatics_directory)
+
+    def hydrostatics_writer(hydrostatics_file_path, kh_file_path, body):
+        """Write the Hydrostatics.dat and KH.dat files"""
+        with open(hydrostatics_file_path, 'w') as hf:
+            for j in range(3):
+                line =  f'XF = {body.center_of_buoyancy[j]:7.4f} - XG = {body.center_of_mass[j]:7.4f} \n'
+                hf.write(line)
+            line = f'Displacement = {body.volume:1.6E}'
+            hf.write(line)
+            hf.close()
+        np.savetxt(kh_file_path, body.hydrostatic_stiffness.values, fmt='%1.6E')
+
+    if isinstance(bodies, FloatingBody):
+        bodies = [bodies]
+    
+    hydrostatics_file_name = "Hydrostatics.dat"
+    kh_file_name = "KH.dat"
+    
+    body_count = len(bodies)
+    if body_count == 1:
+        body = bodies[0]
+        hydrostatics_file_path = os.path.join(hydrostatics_directory, hydrostatics_file_name)
+        kh_file_path = os.path.join(hydrostatics_directory, kh_file_name)
+        hydrostatics_writer(hydrostatics_file_path, kh_file_path, body)
+    else:
+        for (i, body) in enumerate(bodies):
+            hydrostatics_file_path = os.path.join(hydrostatics_directory, f"Hydrostatics_{i}.dat")
+            kh_file_path = os.path.join(hydrostatics_directory, f"KH_{i}.dat")
+            hydrostatics_writer(hydrostatics_file_path, kh_file_path, body)
```

### Comparing `capytaine-1.5.post1/capytaine/io/mesh_loaders.py` & `capytaine-2.0/capytaine/io/mesh_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -693,15 +693,15 @@
     Parameters
     ----------
     filename: str
         name of the mesh file on disk
 
     Returns
     -------
-    Mesh
+    Mesh or ReflectionSymmetricMesh
         the loaded mesh
 
     Note
     ----
     GDF files have a 1-indexing
     """
 
@@ -968,14 +968,70 @@
         faces.append(list(map(int, ifile.readline().split())))
     faces = np.asarray(faces, dtype=int)
     faces -= 1
 
     return Mesh(vertices, faces, name)
 
 
+def load_PNL(filename, name=None):
+    """Load mesh using HAMS file format.
+
+    Parameters
+    ----------
+    filename: str
+        name of the mesh file on disk
+
+    Returns
+    -------
+    Mesh or ReflectionSymmetricMesh
+        the loaded mesh
+    """
+
+    with open(filename, 'r') as f:
+        # Skip 3 title lines
+        f.readline()
+        f.readline()
+        f.readline()
+        # Read header data
+        nb_faces, nb_vertices, x_sym, y_sym = map(int, f.readline().split())
+        # Skip 2 more lines
+        f.readline()
+        f.readline()
+        vertices = np.genfromtxt((f.readline() for _ in range(nb_vertices)), usecols=(1, 2, 3))
+        # Skip 3 more lines
+        f.readline()
+        f.readline()
+        f.readline()
+        faces = np.zeros((nb_faces, 4), dtype=int)
+        for i in range(nb_faces):
+            index, nb_corners, *data = map(int, f.readline().split())
+            assert i+1 == index
+            if nb_corners == 3:  # Triangle
+                assert len(data) == 3
+                faces[i, 0:3] = data
+                faces[i, 3] = faces[i, 2]  # Convention for triangles in Capytaine: repeat last vertex
+            elif int(nb_corners) == 4:  # Quadrangle
+                assert len(data) == 4
+                faces[i, :] = data
+    faces = faces - 1  # Going from Fortran 1-based indices to Numpy 0-based indices
+
+    if x_sym == 1 and y_sym == 0:
+        half_mesh = Mesh(vertices, faces, name=(f"half_of_{name}" if name is not None else None))
+        return ReflectionSymmetricMesh(half_mesh, plane=yOz_Plane, name=name)
+    elif x_sym == 0 and y_sym == 1:
+        half_mesh = Mesh(vertices, faces, name=(f"half_of_{name}" if name is not None else None))
+        return ReflectionSymmetricMesh(half_mesh, plane=xOz_Plane, name=name)
+    elif x_sym == 1 and y_sym == 1:
+        quarter_mesh = Mesh(vertices, faces, name=(f"quarter_of_{name}" if name is not None else None))
+        half_mesh = ReflectionSymmetricMesh(quarter_mesh, plane=xOz_Plane, name=(f"half_of_{name}" if name is not None else None))
+        return ReflectionSymmetricMesh(half_mesh, plane=yOz_Plane, name=name)
+    else:
+        return Mesh(vertices, faces, name)
+
+
 extension_dict = {  # keyword, reader
     'dat': load_MAR,
     'mar': load_MAR,
     'nemoh': load_MAR,
     'wamit': load_GDF,
     'gdf': load_GDF,
     'diodore-inp': load_INP,
@@ -997,9 +1053,11 @@
     'tecplot': load_TEC,
     'tec': load_TEC,
     'med': load_MED,
     'salome': load_MED,
     'vrml': load_WRL,
     'wrl': load_WRL,
     'nem': load_NEM,
-    'nemoh_mesh': load_NEM
+    'nemoh_mesh': load_NEM,
+    'pnl': load_PNL,
+    'hams': load_PNL,
 }
```

### Comparing `capytaine-1.5.post1/capytaine/io/mesh_writers.py` & `capytaine-2.0/capytaine/io/mesh_writers.py`

 * *Files 6% similar despite different names*

```diff
@@ -616,14 +616,54 @@
     raise NotImplementedError('MED writer is not implemented yet')
 
 
 def write_WRL(filename, vertices, faces):
     raise NotImplementedError('VRML writer is not implemented yet')
 
 
+def write_PNL(filename, vertices, faces):
+    """Write a mesh to a file using HAMS file format.
+
+    Took some inspiration from "nemohmesh_to_pnl" by Garett Barter
+    https://github.com/WISDEM/pyHAMS/blob/d10b51122e92849c63640b34e4fa9d413eb306fd/pyhams/pyhams.py#L11
+
+    This writer does not support symmetries.
+
+    Parameters
+    ----------
+    filename: str
+        name of the mesh file to be written on disk
+    vertices: ndarray
+        numpy array of the coordinates of the mesh's nodes
+    faces: ndarray
+        numpy array of the faces' nodes connectivities
+    """
+    with open(filename, 'w') as f:
+        f.write('    --------------Hull Mesh File---------------\n')
+        f.write('\n')
+        f.write('    # Number of Panels, Nodes, X-Symmetry and Y-Symmetry\n')
+        f.write(f'         {faces.shape[0]}         {vertices.shape[0]}         0         0\n')
+        f.write('\n')
+        f.write('    #Start Definition of Node Coordinates     ! node_number   x   y   z\n')
+        for i, vertex in enumerate(vertices):
+            f.write("{:>5}{:>18.6f}{:>18.6f}{:>18.6f}\n".format(i+1, *vertex))
+        f.write('   #End Definition of Node Coordinates\n')
+        f.write('\n')
+        f.write('   #Start Definition of Node Relations   ! panel_number  number_of_vertices   Vertex1_ID   Vertex2_ID   Vertex3_ID   (Vertex4_ID)\n')
+        for i, face in enumerate(faces):
+            face = face + 1
+            if face[2] == face[3]:  # Triangle
+                f.write("{:>5}{:>5}{:>10}{:>10}{:>10}\n".format(i+1, 3, *face[:3]))
+            else:
+                f.write("{:>5}{:>5}{:>10}{:>10}{:>10}{:>10}\n".format(i+1, 4, *face))
+        f.write('   #End Definition of Node Relations\n')
+        f.write('\n')
+        f.write('    --------------End Hull Mesh File---------------\n')
+
+
 extension_dict = {  # keyword,  writer
     'mar': write_MAR,
     'nemoh': write_MAR,
     'wamit': write_GDF,
     'gdf': write_GDF,
     'diodore-inp': write_INP,
     'inp': write_INP,
@@ -644,9 +684,11 @@
     'tecplot': write_TEC,
     'tec': write_TEC,
     'med': write_MED,
     'salome': write_MED,
     'vrml': write_WRL,
     'wrl': write_WRL,
     'nem': write_NEM,
-    'nemoh_mesh': write_NEM
+    'nemoh_mesh': write_NEM,
+    'pnl': write_PNL,
+    'hams': write_PNL,
 }
```

### Comparing `capytaine-1.5.post1/capytaine/io/meshio.py` & `capytaine-2.0/capytaine/io/meshio.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/io/xarray.py` & `capytaine-2.0/capytaine/io/xarray.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 # Copyright (C) 2017-2019 Matthieu Ancellin
 # See LICENSE file at <https://github.com/mancellin/capytaine>
 
 import logging
 from datetime import datetime
 from itertools import product
+from collections import Counter
 from typing import Sequence, List, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from scipy.optimize import newton
 
@@ -60,28 +61,41 @@
         bodies = [bodies]
 
     # SANITY CHECKS
     assert len(list(set(body.name for body in bodies))) == len(bodies), \
         "All bodies should have different names."
 
     # Warn user in case of key with unrecognized name (e.g. mispells)
-    keys_in_dataset = set(dataset.keys()) | set(dataset.coords.keys())
-    accepted_keys = {'wave_direction', 'radiating_dof', 'body_name', 'omega', 'water_depth', 'rho', 'g'}
+    keys_in_dataset = set(dataset.dims.keys())
+    accepted_keys = {'wave_direction', 'radiating_dof', 'influenced_dof',
+                     'body_name', 'omega', 'period', 'wavelength', 'wavenumber',
+                     'water_depth', 'rho', 'g'}
     unrecognized_keys = keys_in_dataset.difference(accepted_keys)
     if len(unrecognized_keys) > 0:
         LOG.warning(f"Unrecognized key(s) in dataset: {unrecognized_keys}")
 
     if ("radiating_dof" not in keys_in_dataset) and ("wave_direction" not in keys_in_dataset):
         raise ValueError("Neither 'radiating_dof' nor 'wave_direction' has been provided in the dataset. "
                 "No linear potential flow problem can be inferred.")
+
+    frequency_keys = keys_in_dataset & {'omega', 'period', 'wavelength', 'wavenumber'}
+    if len(frequency_keys) > 1:
+            raise ValueError("Setting problems requires at most one of the following: omega (angular frequency) OR period OR wavenumber OR wavelength.\n"
+                             "Received {}".format(frequency_keys))
     # END SANITY CHECKS
 
     dataset = _unsqueeze_dimensions(dataset)
 
-    omega_range = dataset['omega'].data if 'omega' in dataset else [_default_parameters['omega']]
+    if len(frequency_keys) == 0:
+        freq_type = "omega"
+        freq_range = [_default_parameters['omega']]
+    else:  # len(frequency_keys) == 1
+        freq_type = list(frequency_keys)[0]  # Get the only item
+        freq_range = dataset[freq_type].data
+
     water_depth_range = dataset['water_depth'].data if 'water_depth' in dataset else [_default_parameters['water_depth']]
     rho_range = dataset['rho'].data if 'rho' in dataset else [_default_parameters['rho']]
     g_range = dataset['g'].data if 'g' in dataset else [_default_parameters['g']]
 
     wave_direction_range = dataset['wave_direction'].data if 'wave_direction' in dataset else None
     radiating_dofs = dataset['radiating_dof'].data.astype(object) if 'radiating_dof' in dataset else None
     # astype(object) is meant to convert Numpy internal string type numpy.str_ to Python general string type.
@@ -92,27 +106,27 @@
         body_range = {body.name: body for body in bodies if body.name in dataset['body_name'].data}
         # Only the bodies listed in the dataset have been kept
     else:
         body_range = {body.name: body for body in bodies}
 
     problems = []
     if wave_direction_range is not None:
-        for omega, wave_direction, water_depth, body_name, rho, g \
-                in product(omega_range, wave_direction_range, water_depth_range, body_range, rho_range, g_range):
+        for freq, wave_direction, water_depth, body_name, rho, g \
+                in product(freq_range, wave_direction_range, water_depth_range, body_range, rho_range, g_range):
             problems.append(
-                DiffractionProblem(body=body_range[body_name], omega=omega,
-                                   wave_direction=wave_direction, sea_bottom=-water_depth, rho=rho, g=g)
+                DiffractionProblem(body=body_range[body_name], **{freq_type: freq},
+                                   wave_direction=wave_direction, water_depth=water_depth, rho=rho, g=g)
             )
 
     if radiating_dofs is not None:
-        for omega, radiating_dof, water_depth, body_name, rho, g \
-                in product(omega_range, radiating_dofs, water_depth_range, body_range, rho_range, g_range):
+        for freq, radiating_dof, water_depth, body_name, rho, g \
+                in product(freq_range, radiating_dofs, water_depth_range, body_range, rho_range, g_range):
             problems.append(
-                RadiationProblem(body=body_range[body_name], omega=omega,
-                                 radiating_dof=radiating_dof, sea_bottom=-water_depth, rho=rho, g=g)
+                RadiationProblem(body=body_range[body_name], **{freq_type: freq},
+                                 radiating_dof=radiating_dof, water_depth=water_depth, rho=rho, g=g)
             )
 
     return sorted(problems)
 
 
 def _squeeze_dimensions(data_array, dimensions=None):
     """Remove dimensions if they are of size 1. The coordinates become scalar coordinates."""
@@ -159,34 +173,22 @@
         Names of dimensions the variables depends on.
         They will appears as dimension in the output dataset only if they have
         more than one different values.
     """
 
     for variable_name in variables:
         df = df[df[variable_name].notnull()].dropna(axis='columns')  # Keep only records with non null values of all the variables
-    df = df.drop_duplicates()
+    df = df.drop_duplicates(optional_dims + dimensions)
     df = df.set_index(optional_dims + dimensions)
 
     da = df.to_xarray()[variables]
     da = _squeeze_dimensions(da, dimensions=optional_dims)
     return da
 
 
-def wavenumber_data_array(results: Sequence[LinearPotentialFlowResult]) -> xr.DataArray:
-    """Read the wavenumbers in a list of :class:`LinearPotentialFlowResult`
-    and store them into a :class:`xarray.DataArray`.
-    """
-    records = pd.DataFrame(
-        [dict(g=result.g, water_depth=result.depth, omega=result.omega, wavenumber=result.wavenumber)
-         for result in results]
-    )
-    ds = _dataset_from_dataframe(records, variables=['wavenumber'], dimensions=['omega'], optional_dims=['g', 'water_depth'])
-    return ds['wavenumber']
-
-
 def hydrostatics_dataset(bodies: Sequence[FloatingBody]) -> xr.Dataset:
     """Create a dataset by looking for 'inertia_matrix' and 'hydrostatic_stiffness'
     for each of the bodies in the list passed as argument.
     """
     dataset = xr.Dataset()
     for body_property in ['inertia_matrix', 'hydrostatic_stiffness']:
         bodies_properties = {body.name: body.__getattribute__(body_property) for body in bodies if hasattr(body, body_property)}
@@ -250,40 +252,44 @@
                 pass
         else:
             for record in result.records:
                 records_list.append(record)
     return records_list
 
 def assemble_dataset(results,
-                     wavenumber=False, wavelength=False, mesh=False, hydrostatics=True,
-                     attrs=None) -> xr.Dataset:
+                     omega=True, wavenumber=True, wavelength=True, period=True,
+                     mesh=False, hydrostatics=True, attrs=None) -> xr.Dataset:
     """Transform a list of :class:`LinearPotentialFlowResult` into a :class:`xarray.Dataset`.
 
     .. todo:: The :code:`mesh` option to store information on the mesh could be improved.
               It could store the full mesh in the dataset to ensure the reproducibility of
               the results.
 
     Parameters
     ----------
     results: list of LinearPotentialFlowResult
         The results that will be read.
+    omega: bool, optional
+        If True, the coordinate 'omega' will be added to the output dataset.
     wavenumber: bool, optional
         If True, the coordinate 'wavenumber' will be added to the output dataset.
     wavelength: bool, optional
         If True, the coordinate 'wavelength' will be added to the output dataset.
+    period: bool, optional
+        If True, the coordinate 'period' will be added to the output dataset.
     mesh: bool, optional
         If True, store some infos on the mesh in the output dataset.
     hydrostatics: bool, optional
         If True, store the hydrostatic data in the output dataset if they exist.
     attrs: dict, optional
         Attributes that should be added to the output dataset.
     """
     dataset = xr.Dataset()
 
-    error_msg = 'results must be either of type LinearPotentialFlowResult or a bemio.io object'
+    error_msg = 'The first argument of `assemble_dataset` must be either a list of LinearPotentialFlowResult or a bemio.io object'
     if hasattr(results, '__iter__'):
         try:
             if 'capytaine' in results[0].__module__:
                 bemio_import = False
             else:
                 raise TypeError(error_msg)
         except:
@@ -293,22 +299,24 @@
         try:
             if 'bemio.io' in results.__module__:
                 bemio_import = True
             else:
                 raise TypeError(error_msg)
         except:
             raise TypeError(error_msg)
-    
+
     if bemio_import:
         records = dataframe_from_bemio(results, wavenumber, wavelength) # TODO add hydrostatics
         all_dofs_in_order = {'Surge': None, 'Sway': None, 'Heave': None, 'Roll': None, 'Pitch': None, 'Yaw': None}
+        main_freq_type = "omega"
 
     else:
         records = pd.DataFrame(collect_records(results))
         all_dofs_in_order = {k: None for r in results for k in r.body.dofs.keys()}
+        main_freq_type = Counter((res.provided_freq_type for res in results)).most_common(1)[0][0]
 
     if attrs is None:
         attrs = {}
     attrs['creation_of_dataset'] = datetime.now().isoformat()
     if len(records) == 0:
         raise ValueError("No result passed to assemble_dataset.")
 
@@ -321,55 +329,80 @@
     optional_dims = ['g', 'rho', 'body_name', 'water_depth']
 
     # RADIATION RESULTS
     if 'added_mass' in records.columns:
         radiation_cases = _dataset_from_dataframe(
             records,
             variables=['added_mass', 'radiation_damping'],
-            dimensions=['omega', 'radiating_dof', 'influenced_dof'],
+            dimensions=[main_freq_type, 'radiating_dof', 'influenced_dof'],
             optional_dims=optional_dims)
+        radiation_cases.added_mass.attrs['long_name'] = 'Added mass'
+        radiation_cases.radiation_damping.attrs['long_name'] = 'Radiation damping'
+        radiation_cases.radiating_dof.attrs['long_name'] = 'Radiating DOF'
+        radiation_cases.influenced_dof.attrs['long_name'] = 'Influenced DOF'
         dataset = xr.merge([dataset, radiation_cases])
 
     # DIFFRACTION RESULTS
     if 'diffraction_force' in records.columns:
-        conventions = set(records['convention'].dropna())
-        if len(conventions) > 1:
-            LOG.warning("Assembling a dataset mixing several conventions.")
-        else:
-            attrs['incoming_waves_convention'] = conventions.pop()
-
         diffraction_cases = _dataset_from_dataframe(
             records,
             variables=['diffraction_force', 'Froude_Krylov_force'],
-            dimensions=['omega', 'wave_direction', 'influenced_dof'],
+            dimensions=[main_freq_type, 'wave_direction', 'influenced_dof'],
             optional_dims=optional_dims)
+        diffraction_cases.diffraction_force.attrs['long_name'] = 'Diffraction force'
+        diffraction_cases.Froude_Krylov_force.attrs['long_name'] = 'Froude Krylov force'
+        diffraction_cases.influenced_dof.attrs['long_name'] = 'Influenced DOF'
+        diffraction_cases.wave_direction.attrs['long_name'] = 'Wave direction'
+        diffraction_cases.wave_direction.attrs['units'] = 'rad'
         dataset = xr.merge([dataset, diffraction_cases])
 
-    # WAVENUMBER
-    if wavenumber:
-        if bemio_import:
-            wavenumber_ds = _dataset_from_dataframe(
-                records.drop_duplicates(subset=['omega']),
+    # OTHER FREQUENCIES TYPES
+    if omega and main_freq_type != "omega":
+        omega_ds = _dataset_from_dataframe(
+                records,
+                variables=['omega'],
+                dimensions=[main_freq_type],
+                optional_dims=['g', 'water_depth'] if main_freq_type in {'wavelength', 'wavenumber'} else []
+                )
+        dataset.coords['omega'] = omega_ds['omega']
+        dataset.omega.attrs['long_name'] = 'Angular frequency'
+        dataset.omega.attrs['units'] = 'rad/s'
+
+    if period and main_freq_type != "period":
+        period_ds = _dataset_from_dataframe(
+                records,
+                variables=['period'],
+                dimensions=[main_freq_type],
+                optional_dims=['g', 'water_depth'] if main_freq_type in {'wavelength', 'wavenumber'} else []
+                )
+        dataset.coords['period'] = period_ds['period']
+        dataset.period.attrs['long_name'] = 'Period'
+        dataset.period.attrs['units'] = 's'
+
+    if wavenumber and main_freq_type != "wavenumber":
+        wavenumber_ds = _dataset_from_dataframe(
+                records,
                 variables=['wavenumber'],
-                dimensions=['omega'],
-                optional_dims=['g', 'water_depth'])
-            dataset.coords['wavenumber'] = wavenumber_ds['wavenumber']
-        else:
-            dataset.coords['wavenumber'] = wavenumber_data_array(results)
-
-    if wavelength:
-        if bemio_import:
-            wavelength_ds = _dataset_from_dataframe(
-                    records.drop_duplicates(subset=['omega']),
-                    variables=['wavelength'],
-                    dimensions=['omega'],
-                    optional_dims=['g', 'water_depth'])
-            dataset.coords['wavelength'] = wavelength_ds['wavelength']
-        else:
-            dataset.coords['wavelength'] = 2*np.pi/wavenumber_data_array(results)
+                dimensions=[main_freq_type],
+                optional_dims=['g', 'water_depth'] if main_freq_type in {'period', 'omega'} else []
+                )
+        dataset.coords['wavenumber'] = wavenumber_ds['wavenumber']
+        dataset.wavenumber.attrs['long_name'] = 'Angular wavenumber'
+        dataset.wavenumber.attrs['units'] = 'rad/m'
+
+    if wavelength and main_freq_type != "wavelength":
+        wavelength_ds = _dataset_from_dataframe(
+                records,
+                variables=['wavelength'],
+                dimensions=[main_freq_type],
+                optional_dims=['g', 'water_depth'] if main_freq_type in {'period', 'omega'} else []
+                )
+        dataset.coords['wavelength'] = wavelength_ds['wavelength']
+        dataset.wavelength.attrs['long_name'] = 'Wave length'
+        dataset.wavelength.attrs['units'] = 'm'
 
     if mesh:
         if bemio_import:
             LOG.warning('Bemio data does not include mesh data. mesh=True is ignored.')
         else:
             # TODO: Store full mesh...
             bodies = list({result.body for result in results})  # Filter out duplicate bodies in the list of results
```

### Comparing `capytaine-1.5.post1/capytaine/matrices/__init__.py` & `capytaine-2.0/capytaine/matrices/__init__.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/matrices/block.py` & `capytaine-2.0/capytaine/matrices/block.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,22 +206,22 @@
     @property
     def stored_data_size(self):
         """Return the number of entries actually stored in memory."""
         size = 0
         for line in self._stored_blocks:
             for block in line:
                 if isinstance(block, np.ndarray):
-                    size += np.product(block.shape)
+                    size += np.prod(block.shape)
                 else:
                     size += block.stored_data_size
         return size
 
     @property
     def density(self):
-        return self.stored_data_size/np.product(self.shape)
+        return self.stored_data_size/np.prod(self.shape)
 
     @property
     def sparcity(self):
         return 1 - self.density
 
     def __hash__(self):
         # Temporary
@@ -461,14 +461,17 @@
         if not hasattr(self, '_str'):
             args = [self.str_shape]
             if self.dtype not in [np.float64, float]:
                 args.append(f"dtype={self.dtype}")
             self._str = f"{self.__class__.__name__}(" + ", ".join(args) + ")"
         return self._str
 
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__str__())
+
     display_color = cycle([f'C{i}' for i in range(10)])
 
     def _patches(self,
                  global_frame: Union[Tuple[int, int], np.ndarray]
                  ):
         """Helper function for displaying the shape of the matrix.
         Recursively returns a list of rectangles representing the sub-blocks of the matrix.
```

### Comparing `capytaine-1.5.post1/capytaine/matrices/block_toeplitz.py` & `capytaine-2.0/capytaine/matrices/block_toeplitz.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/matrices/builders.py` & `capytaine-2.0/capytaine/matrices/builders.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/matrices/linear_solvers.py` & `capytaine-2.0/capytaine/matrices/linear_solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """Solve linear system with the LU decomposition.
 
     The latest LU decomposition is kept in memory, if a system with the same matrix needs to be solved again, then the decomposition is reused.
 
     Most of the complexity of this class comes from:
     1. @lru_cache does not work because numpy arrays are not hashable. So a basic cache system has been recoded from scratch.
     2. To be the default solver for the BasicMatrixEngine, the solver needs to support matrices for problems with one or two reflection symmetries.
-       Hence, a custom way to cache the LU decomposition of the matrices involved in the direct linear resolution of the symmetric problem.
+    Hence, a custom way to cache the LU decomposition of the matrices involved in the direct linear resolution of the symmetric problem.
     """
     def __init__(self):
         self.cached_matrix = None
         self.cached_decomp = None
 
     def solve(self, A, b):
         return self.solve_with_decomp(self.cached_lu_decomp(A), b)
```

### Comparing `capytaine-1.5.post1/capytaine/matrices/low_rank.py` & `capytaine-2.0/capytaine/matrices/low_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,19 +321,19 @@
             return self.left_matrix @ self.right_matrix
 
     def __array__(self, dtype=None):
         return self.full_matrix(dtype=dtype)
 
     @property
     def stored_data_size(self):
-        return np.product(self.left_matrix.shape) + np.product(self.right_matrix.shape)
+        return np.prod(self.left_matrix.shape) + np.prod(self.right_matrix.shape)
 
     @property
     def density(self):
-        return self.stored_data_size/np.product(self.shape)
+        return self.stored_data_size/np.prod(self.shape)
 
     @property
     def sparcity(self):
         return 1 - self.density
 
     ####################
     #  Transformation  #
```

### Comparing `capytaine-1.5.post1/capytaine/meshes/clipper.py` & `capytaine-2.0/capytaine/meshes/clipper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 from capytaine.meshes.geometry import Plane
 from capytaine.meshes.meshes import Mesh
 
 LOG = logging.getLogger(__name__)
 
 
-def clip(source_mesh: Mesh, plane: Plane, vicinity_tol=1e-3, name=None):
+def clip(source_mesh: Mesh, plane: Plane, vicinity_tol=1e-12, name=None):
     """Return a new mesh containing the source mesh clipped by the plane.
 
     Parameters
     ----------
     source_mesh : Mesh
         The mesh to be clipped.
     plane : Plane, optional
         The clipping plane.
     vicinity_tol : float, optional
-        The absolute tolerance to consider en vertex is on the plane. Default is 1e-3.
+        The absolute tolerance to consider en vertex is on the plane. Default is 1e-12.
     name: string, optional
         A name for the new clipped mesh.
     """
     vertices_data = _vertices_positions_wrt_plane(source_mesh, plane, vicinity_tol)
 
     nb_vertices_above_or_on_plane = np.count_nonzero(
         vertices_data['vertices_above_mask'] | vertices_data['vertices_on_mask']
```

### Comparing `capytaine-1.5.post1/capytaine/meshes/collections.py` & `capytaine-2.0/capytaine/meshes/collections.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 import reprlib
 from itertools import chain, accumulate
 from functools import lru_cache
 from typing import Iterable, Union
 
 import numpy as np
 
-from capytaine.meshes.geometry import Abstract3DObject, inplace_transformation
+from capytaine.meshes.geometry import Abstract3DObject, ClippableMixin, inplace_transformation
 from capytaine.meshes.surface_integrals import SurfaceIntegralsMixin
 from capytaine.meshes.meshes import Mesh
 
 LOG = logging.getLogger(__name__)
 
 
-class CollectionOfMeshes(SurfaceIntegralsMixin, Abstract3DObject):
+class CollectionOfMeshes(ClippableMixin, SurfaceIntegralsMixin, Abstract3DObject):
     """A tuple of meshes.
     It gives access to all the vertices of all the sub-meshes as if it were a mesh itself.
     Collections can be nested to store meshes in a tree structure.
 
     Parameters
     ----------
     meshes: Iterable of Mesh or CollectionOfMeshes
@@ -49,14 +49,17 @@
         reprer.maxother = 100
         meshes_names = reprer.repr(self._meshes)
         if self.name is not None:
             return f"{self.__class__.__name__}({meshes_names}, name={self.name})"
         else:
             return f"{self.__class__.__name__}{meshes_names}"
 
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__repr__())
+
     def __str__(self):
         if self.name is not None:
             return self.name
         else:
             return repr(self)
 
     def __iter__(self):
@@ -248,33 +251,20 @@
         faces_shifts = list(accumulate(chain([0], (mesh.nb_faces for mesh in self[:-1]))))
         for mesh, faces_shift in zip(self, faces_shifts):
             mesh.clip(plane)
             self._clipping_data['faces_ids'].extend([i + faces_shift for i in mesh._clipping_data['faces_ids']])
         self._clipping_data['faces_ids'] = np.asarray(self._clipping_data['faces_ids'])
         self.prune_empty_meshes()
 
-    def clipped(self, plane, **kwargs):
-        # Same API as for the other transformations
-        return self.clip(plane, inplace=False, **kwargs)
-
     def symmetrized(self, plane):
         from capytaine.meshes.symmetric import ReflectionSymmetricMesh
         half = self.clipped(plane, name=f"{self.name}_half")
         return ReflectionSymmetricMesh(half, plane=plane, name=f"symmetrized_of_{self.name}")
 
     @inplace_transformation
-    def keep_immersed_part(self, **kwargs):
-        for mesh in self:
-            mesh.keep_immersed_part(**kwargs)
-        self.prune_empty_meshes()
-
-    def immersed_part(self, free_surface=0.0, sea_bottom=-np.infty):
-        return self.keep_immersed_part(free_surface, sea_bottom, inplace=False)
-
-    @inplace_transformation
     def prune_empty_meshes(self):
         """Remove empty meshes from the collection."""
         self._meshes = tuple(mesh for mesh in self if mesh.nb_faces > 0 and mesh.nb_vertices > 0)
 
     @property
     def axis_aligned_bbox(self):
         """Get the axis aligned bounding box of the mesh.
```

### Comparing `capytaine-1.5.post1/capytaine/meshes/geometry.py` & `capytaine-2.0/capytaine/meshes/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """Tools to describe geometric objects in 3D.
 Based on meshmagick <https://github.com/LHEEA/meshmagick> by François Rongère.
 """
 # Copyright (C) 2017-2019 Matthieu Ancellin, based on the work of François Rongère
 # See LICENSE file at <https://github.com/mancellin/capytaine>
 
 from abc import ABC, abstractmethod
+from capytaine.tools.deprecation_handling import _get_water_depth
 
 import numpy as np
 
 e_x = np.array((1, 0, 0))
 e_y = np.array((0, 1, 0))
 e_z = np.array((0, 0, 1))
 
@@ -133,14 +134,43 @@
     def rotated_z(self, *args, **kwargs):
         return self.rotate_z(*args, inplace=False, **kwargs)
 
     def rotated_around_center_to_align_vectors(self, *args, **kwargs):
         return self.rotate_around_center_to_align_vectors(*args, inplace=False, **kwargs)
 
 
+class ClippableMixin(ABC):
+    """Abstract base class for object that can be clipped.
+    The child classes should inplement a `clip` method, then this abstract
+    class will append the new methods `clipped`, `keep_immersed_part` and
+    `immersed_part`, all based on `clip`.
+    """
+
+    @abstractmethod
+    def clip(self, plane):
+        pass
+
+    def clipped(self, plane, **kwargs):
+        # Same API as for the other transformations
+        return self.clip(plane, inplace=False, **kwargs)
+
+    @inplace_transformation
+    def keep_immersed_part(self, free_surface=0.0, *, sea_bottom=None, water_depth=None):
+        self.clip(Plane(normal=(0, 0, 1), point=(0, 0, free_surface)))
+        water_depth = _get_water_depth(free_surface, water_depth, sea_bottom,
+                                       default_water_depth=np.infty)
+        if water_depth < np.infty:
+            self.clip(Plane(normal=(0, 0, -1), point=(0, 0, free_surface-water_depth)))
+        return self
+
+    def immersed_part(self, free_surface=0.0, *, sea_bottom=None, water_depth=None):
+        return self.keep_immersed_part(free_surface, inplace=False, name=self.name,
+                                       sea_bottom=sea_bottom, water_depth=water_depth)
+
+
 ######################
 #  HELPER FUNCTIONS  #
 ######################
 
 def orthogonal_vectors(vec1, vec2) -> bool:
     return np.linalg.norm(vec1 @ vec2) < 1e-6
 
@@ -295,14 +325,19 @@
             raise NotImplementedError
 
     @property
     def c(self):
         """Distance from plane to origin."""
         return np.linalg.norm(self.normal @ self.point)
 
+    @property
+    def s(self):
+        """Distance from origin to plane along the normal"""
+        return np.dot(self.normal, self.point)
+
     #################################
     #  Transformation of the plane  #
     #################################
 
     def copy(self, name=None):
         return Plane(normal=self.normal.copy(), point=self.point.copy())
 
@@ -361,15 +396,15 @@
         I : ndarray
             Coordinates of intersection point
         """
         assert len(p0) == 3 and len(p1) == 3
 
         p0n = np.dot(p0, self.normal)
         p1n = np.dot(p1, self.normal)
-        t = (p0n - self.c) / (p0n - p1n)
+        t = (p0n - self.s) / (p0n - p1n)
         if t < 0. or t > 1.:
             raise RuntimeError('Intersection is outside the edge')
         return (1-t) * p0 + t * p1
 
 
 yOz_Plane = Plane(normal=e_x, point=(0, 0, 0))
 xOz_Plane = Plane(normal=e_y, point=(0, 0, 0))
```

### Comparing `capytaine-1.5.post1/capytaine/meshes/meshes.py` & `capytaine-2.0/capytaine/meshes/meshes.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 import logging
 from itertools import count
 
 import numpy as np
 from numpy.linalg import norm
 
-from capytaine.meshes.geometry import Abstract3DObject, Plane, inplace_transformation
-from capytaine.meshes.properties import compute_faces_properties, compute_connectivity
-from capytaine.meshes.surface_integrals import compute_faces_integrals, SurfaceIntegralsMixin
+from capytaine.meshes.geometry import Abstract3DObject, ClippableMixin, Plane, inplace_transformation
+from capytaine.meshes.properties import compute_faces_properties
+from capytaine.meshes.surface_integrals import SurfaceIntegralsMixin
 from capytaine.meshes.quality import (merge_duplicates, heal_normals, remove_unused_vertices,
                                       heal_triangles, remove_degenerated_faces)
 from capytaine.tools.optional_imports import import_optional_dependency
 
 LOG = logging.getLogger(__name__)
 
 
-class Mesh(SurfaceIntegralsMixin, Abstract3DObject):
+class Mesh(ClippableMixin, SurfaceIntegralsMixin, Abstract3DObject):
     """A class to handle unstructured 2D meshes in a 3D space.
 
     Parameters
     ----------
     vertices : array_like of shape (nv, 3)
         Array of mesh vertices coordinates.Each line of the array represents one vertex
         coordinates
@@ -62,14 +62,17 @@
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return (f"{self.__class__.__name__}(nb_vertices={self.nb_vertices}, "
                 f"nb_faces={self.nb_faces}, name={self.name})")
 
+    def _repr_pretty_(self, p, cycle):
+        p.text(self.__repr__())
+
     @property
     def nb_vertices(self) -> int:
         """Get the number of vertices in the mesh."""
         return self._vertices.shape[0]
 
     @property
     def vertices(self) -> np.ndarray:
@@ -160,15 +163,15 @@
         if self.is_triangle(face_id):
             return self._faces[face_id, :3]
         else:
             return self._faces[face_id]
 
     def extract_one_face(self, id_face):
         vertices = self.vertices[self.faces[id_face, :], :]
-        mesh = SingleFace(vertices)
+        mesh = Mesh(vertices=vertices, faces=np.array([[0, 1, 2, 3]]), name=f"single_face_from_{self.name}")
 
         for prop in self.__internals__:
             if prop[:4] == "face":
                 mesh.__internals__[prop] = self.__internals__[prop][[id_face]]
 
         return mesh
 
@@ -518,27 +521,27 @@
             faces.append(vertices)
 
         if color_field is None:
             if 'facecolors' not in kwargs:
                 kwargs['facecolors'] = "yellow"
         else:
             if cmap is None:
-                cmap = cm.get_cmap('coolwarm')
+                cmap = matplotlib.colormaps['coolwarm']
             m = cm.ScalarMappable(cmap=cmap)
             m.set_array([min(color_field), max(color_field)])
             m.set_clim(vmin=min(color_field), vmax=max(color_field))
             colors = m.to_rgba(color_field)
             kwargs['facecolors'] = colors
         if 'edgecolor' not in kwargs:
             kwargs['edgecolor'] = 'k'
 
         ax.add_collection3d(Poly3DCollection(faces, **kwargs))
 
         if color_field is not None:
-            cbar = plt.colorbar(m)
+            cbar = plt.colorbar(m, ax=ax)
             if cbar_label is not None:
                 cbar.set_label(cbar_label)
 
 
 
         # Plot normal vectors.
         if normal_vectors:
@@ -631,30 +634,14 @@
         from capytaine.meshes.clipper import clip
         clipped_self = clip(self, plane=plane)
         self.vertices = clipped_self.vertices
         self.faces = clipped_self.faces
         self._clipping_data = clipped_self._clipping_data
         return self
 
-    def clipped(self, plane, **kwargs) -> 'Mesh':
-        # Same API as for the other transformations
-        return self.clip(plane, inplace=False, **kwargs)
-
-    @inplace_transformation
-    def keep_immersed_part(self, free_surface=0.0, sea_bottom=-np.infty):
-        """Clip the mesh with two horizontal planes corresponding
-        with the free surface and the sea bottom."""
-        self.clip(Plane(normal=(0, 0, 1), point=(0, 0, free_surface)))
-        if sea_bottom > -np.infty:
-            self.clip(Plane(normal=(0, 0, -1), point=(0, 0, sea_bottom)))
-        return self
-
-    def immersed_part(self, free_surface=0.0, sea_bottom=-np.infty):
-        return self.keep_immersed_part(free_surface, sea_bottom, inplace=False, name=self.name)
-
     @inplace_transformation
     def triangulate_quadrangles(self) -> 'Mesh':
         """Triangulates every quadrangles of the mesh by simple splitting.
         Each quadrangle gives two triangles.
 
         Note
         ----
@@ -786,104 +773,7 @@
         self.remove_degenerated_faces()
         self.merge_duplicates()
         self.heal_triangles()
         if closed_mesh:
             self.heal_normals()
         return self
 
-    #################
-    #  Edges stats  #
-    #################
-
-    def _edges_stats(self):
-        """Computes the min, max, and mean of the mesh's edge length"""
-        vertices = self.vertices[self.faces]
-        edge_length = np.zeros((self.nb_faces, 4), dtype=float)
-        for i in range(4):
-            edge = vertices[:, i, :] - vertices[:, i-1, :]
-            edge_length[:, i] = np.sqrt(np.einsum('ij, ij -> i', edge, edge))
-
-        return edge_length.min(), edge_length.max(), edge_length.mean()
-
-    @property
-    def min_edge_length(self) -> float:
-        """The mesh's minimum edge length"""
-        return self._edges_stats()[0]
-
-    @property
-    def max_edge_length(self) -> float:
-        """The mesh's maximum edge length"""
-        return self._edges_stats()[1]
-
-    @property
-    def mean_edge_length(self) -> float:
-        """The mesh's mean edge length"""
-        return self._edges_stats()[2]
-
-    #######################
-    #  Surface integrals  #
-    #######################
-
-    def get_surface_integrals(self) -> np.ndarray:
-        """Get the mesh surface integrals."""
-        if 'surface_integrals' not in self.__internals__:
-            self.__internals__['surface_integrals'] = compute_faces_integrals(self)
-        return self.__internals__['surface_integrals']
-
-    @property
-    def volume(self) -> float:
-        """Get the mesh enclosed volume."""
-        normals = self.faces_normals
-        sigma_0_2 = self.get_surface_integrals()[:3]
-
-        return (normals.T * sigma_0_2).sum() / 3.
-
-    ####################
-    #  Connectivities  #
-    ####################
-
-    @property
-    def vv(self) -> dict:
-        """Get the vertex / vertex connectivity dictionary."""
-        if 'v_v' not in self.__internals__:
-            self.__internals__.update(compute_connectivity(self))
-        return self.__internals__['v_v']
-
-    @property
-    def vf(self) -> dict:
-        """Get the vertex / faces connectivity dictionary."""
-        if 'v_f' not in self.__internals__:
-            self.__internals__.update(compute_connectivity(self))
-        return self.__internals__['v_f']
-
-    @property
-    def ff(self) -> dict:
-        """Get the face / faces connectivity dictionary."""
-        if 'f_f' not in self.__internals__:
-            self.__internals__.update(compute_connectivity(self))
-        return self.__internals__['f_f']
-
-    @property
-    def boundaries(self) -> list:
-        """Get a list that stores lists of boundary connected vertices."""
-        if 'boundaries' not in self.__internals__:
-            self.__internals__.update(compute_connectivity(self))
-        return self.__internals__['boundaries']
-
-    @property
-    def nb_boundaries(self) -> int:
-        """Get the number of boundaries in the mesh."""
-        if 'boundaries' not in self.__internals__:
-            self.__internals__.update(compute_connectivity(self))
-        return len(self.__internals__['boundaries'])
-
-
-class SingleFace(Mesh):
-    """A view on a single face of a mesh.
-    To be used for ACA."""
-
-    _faces = np.arange(4).reshape((1, 4))
-    name = "some single face"
-
-    def __init__(self, vertices=None):
-        self._vertices = vertices
-        self.__internals__ = dict()
```

### Comparing `capytaine-1.5.post1/capytaine/meshes/predefined/cylinders.py` & `capytaine-2.0/capytaine/meshes/predefined/cylinders.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/meshes/predefined/rectangles.py` & `capytaine-2.0/capytaine/meshes/predefined/rectangles.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/meshes/predefined/spheres.py` & `capytaine-2.0/capytaine/meshes/predefined/spheres.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/meshes/properties.py` & `capytaine-2.0/capytaine/meshes/properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,27 +27,45 @@
     # Collectively dealing with triangles
     # triangles = _faces[triangle_mask]
     triangles_id = mesh.triangles_ids
     triangles = mesh._faces[triangles_id]
 
     triangles_normals = np.cross(mesh._vertices[triangles[:, 1]] - mesh._vertices[triangles[:, 0]],
                                  mesh._vertices[triangles[:, 2]] - mesh._vertices[triangles[:, 0]])
-    triangles_areas = np.linalg.norm(triangles_normals, axis=1)
-    faces_normals[triangles_id] = triangles_normals / np.array(([triangles_areas, ] * 3)).T
-    faces_areas[triangles_id] = triangles_areas / 2.
+    triangles_normals_norm = np.linalg.norm(triangles_normals, axis=1)
+
+    degenerate_triangle = np.abs(triangles_normals_norm) < 1e-12
+    triangles_id = triangles_id[~degenerate_triangle]
+    triangles_normals = triangles_normals[~degenerate_triangle, :]
+    triangles_normals_norm = triangles_normals_norm[~degenerate_triangle]
+    triangles = triangles[~degenerate_triangle, :]
+    # Now, continue the computations without the degenerate triangles
+
+    faces_normals[triangles_id] = triangles_normals / triangles_normals_norm[:, np.newaxis]
+    faces_areas[triangles_id] = triangles_normals_norm / 2.
     faces_centers[triangles_id] = np.sum(mesh._vertices[triangles[:, :3]], axis=1) / 3.
 
     # Collectively dealing with quads
     quads_id = mesh.quadrangles_ids
     quads = mesh._faces[quads_id]
     # quads = _faces[quads_mask]
 
     quads_normals = np.cross(mesh._vertices[quads[:, 2]] - mesh._vertices[quads[:, 0]],
                              mesh._vertices[quads[:, 3]] - mesh._vertices[quads[:, 1]])
-    faces_normals[quads_id] = quads_normals / np.array(([np.linalg.norm(quads_normals, axis=1), ] * 3)).T
+
+    quads_normals_norm = np.linalg.norm(quads_normals, axis=1)
+
+    degenerate_quad = np.abs(quads_normals_norm) < 1e-12
+    quads_id = quads_id[~degenerate_quad]
+    quads_normals = quads_normals[~degenerate_quad]
+    quads_normals_norm = quads_normals_norm[~degenerate_quad]
+    quads = quads[~degenerate_quad, :]
+    # Now, continue the computations without the degenerate quads
+
+    faces_normals[quads_id] = quads_normals / quads_normals_norm[:, np.newaxis]
 
     a1 = np.linalg.norm(np.cross(mesh._vertices[quads[:, 1]] - mesh._vertices[quads[:, 0]],
                                  mesh._vertices[quads[:, 2]] - mesh._vertices[quads[:, 0]]), axis=1) * 0.5
     a2 = np.linalg.norm(np.cross(mesh._vertices[quads[:, 3]] - mesh._vertices[quads[:, 0]],
                                  mesh._vertices[quads[:, 2]] - mesh._vertices[quads[:, 0]]), axis=1) * 0.5
     faces_areas[quads_id] = a1 + a2
 
@@ -176,8 +194,8 @@
                     break
         except KeyError:
             break
 
     return {'v_v': v_v,
             'v_f': v_f,
             'f_f': f_f,
-            'boundaries': boundaries}
+            'boundaries': boundaries}
```

### Comparing `capytaine-1.5.post1/capytaine/meshes/quality.py` & `capytaine-2.0/capytaine/meshes/quality.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # See LICENSE file at <https://github.com/mancellin/capytaine>
 
 import logging
 
 import numpy as np
 
 from capytaine.meshes.geometry import inplace_transformation
+from capytaine.meshes.properties import compute_connectivity
 
 LOG = logging.getLogger(__name__)
 
 
 def merge_duplicates(mesh, atol=1e-8):
     """Merges the duplicate vertices of the mesh in place.
 
@@ -159,18 +160,19 @@
     # TODO: return the different groups of a mesh in case it is made of several unrelated groups
 
     nv = mesh.nb_vertices
     nf = mesh.nb_faces
     faces = mesh._faces
 
     # Building connectivities
-    v_v = mesh.vv
-    v_f = mesh.vf
-    f_f = mesh.ff
-    boundaries = mesh.boundaries
+    connectivities = compute_connectivity(mesh)
+    v_v = connectivities["v_v"]
+    v_f = connectivities["v_f"]
+    f_f = connectivities["f_f"]
+    boundaries = connectivities["boundaries"]
 
     if len(boundaries) > 0:
         mesh_closed = False
     else:
         mesh_closed = True
 
     # Flooding the mesh to find inconsistent normals
```

### Comparing `capytaine-1.5.post1/capytaine/meshes/symmetric.py` & `capytaine-2.0/capytaine/meshes/symmetric.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/post_pro/free_surfaces.py` & `capytaine-2.0/capytaine/post_pro/free_surfaces.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/post_pro/impedance.py` & `capytaine-2.0/capytaine/post_pro/impedance.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,24 +54,24 @@
         H = H + stiffness
 
     return H
 
 
 def impedance(dataset, dissipation=None, stiffness=None):
     """Complex-valued mechanical impedance matrix.
-    See Falnes for more theoretical details.
+    See Falnes for more theoretical details::
 
-    @book{falnes2002ocean,
-          title={Ocean Waves and Oscillating Systems: Linear Interactions Including Wave-Energy Extraction},
-          author={Falnes, J.},
-          isbn={9781139431934},
-          url={https://books.google.com/books?id=bl1FyQjCklgC},
-          year={2002},
-          publisher={Cambridge University Press}
-    }
+        @book{falnes2002ocean,
+              title={Ocean Waves and Oscillating Systems: Linear Interactions Including Wave-Energy Extraction},
+              author={Falnes, J.},
+              isbn={9781139431934},
+              url={https://books.google.com/books?id=bl1FyQjCklgC},
+              year={2002},
+              publisher={Cambridge University Press}
+        }
 
     Parameters
     ----------
     dataset: xarray Dataset
         The hydrodynamical dataset.
         This function supposes that variables named 'inertia_matrix' and 'hydrostatic_stiffness' are in the dataset.
         Other variables can be computed by Capytaine, by those two should be manually added to the dataset.
```

### Comparing `capytaine-1.5.post1/capytaine/post_pro/kochin.py` & `capytaine-2.0/capytaine/post_pro/kochin.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     if result.sources is None:
         raise Exception(f"""The values of the sources of {result} cannot been found.
         They probably have not been stored by the solver because the option keep_details=True have not been set.
         Please re-run the resolution with this option.""")
 
     k = result.wavenumber
-    h = result.depth
+    h = result.water_depth
 
     # omega_bar.shape = (nb_faces, 2) @ (2, nb_theta)
     omega_bar = (result.body.mesh.faces_centers[:, 0:2] - ref_point) @ (np.cos(theta), np.sin(theta))
 
     if 0 <= k*h < 20:
         cih = np.cosh(k*(result.body.mesh.faces_centers[:, 2]+h))/np.cosh(k*h)
     else:
```

### Comparing `capytaine-1.5.post1/capytaine/post_pro/rao.py` & `capytaine-2.0/capytaine/post_pro/rao.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,23 +39,28 @@
     """
 
     # ASSEMBLE MATRICES
     H = rao_transfer_function(dataset, dissipation, stiffness)
 
     LOG.info("Compute RAO.")
 
-    omega = dataset.coords['omega']  # Range of frequencies in the dataset
+    freq_dims = set(dataset.dims) & {'omega', 'period', 'wavelength', 'wavenumber'}
+    if len(freq_dims) != 1:
+        raise ValueError("The dataset provided to compute the RAO should one (and only one) dimension" +
+                         " among the following: 'omega', 'period', 'wavelength' or 'wavenumber'\n" +
+                         f"The received dataset has the following dimensions: {dataset.dims}")
+    main_freq_type = freq_dims.pop()
 
     if 'excitation_force' not in dataset:
         dataset['excitation_force'] = dataset['Froude_Krylov_force'] + dataset['diffraction_force']
     excitation = dataset['excitation_force'].sel(wave_direction=wave_direction)
 
     # SOLVE LINEAR SYSTEMS
     # Reorder dimensions of the arrays to be sure to solve the right system.
-    H = H.transpose('omega', 'radiating_dof', 'influenced_dof')
-    excitation = excitation.transpose('omega',  'influenced_dof')
+    H = H.transpose(main_freq_type, 'radiating_dof', 'influenced_dof')
+    excitation = excitation.transpose(main_freq_type,  'influenced_dof')
 
     # Solve the linear systems (one for each value of omega)
     X = np.linalg.solve(H, excitation)
 
-    return xr.DataArray(X, coords=[omega, dataset.coords['radiating_dof']], dims=['omega', 'radiating_dof'])
+    return xr.DataArray(X, coords=[dataset.coords[main_freq_type], dataset.coords['radiating_dof']], dims=[main_freq_type, 'radiating_dof'])
```

### Comparing `capytaine-1.5.post1/capytaine/tools/lru_cache.py` & `capytaine-2.0/capytaine/tools/lru_cache.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/tools/optional_imports.py` & `capytaine-2.0/capytaine/tools/optional_imports.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/tools/prony_decomposition.py` & `capytaine-2.0/capytaine/tools/prony_decomposition.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/ui/cli.py` & `capytaine-2.0/capytaine/ui/cli.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/ui/vtk/animation.py` & `capytaine-2.0/capytaine/ui/vtk/animation.py`

 * *Files 15% similar despite different names*

```diff
@@ -294,61 +294,16 @@
         del image_filter
         del writer
         del render_window
 
     def embed_in_notebook(self, resolution=(640, 360), **kwargs):
         from tempfile import mkstemp
         from IPython.core.display import Video
-
-        class CustomIPythonVideo(Video):
-            def __init__(self, *args, html_attributes="controls", **kwargs):
-                self.html_attributes = html_attributes
-                super(CustomIPythonVideo, self).__init__(*args, **kwargs)
-
-            def _repr_html_(self):
-                import mimetypes
-                from binascii import b2a_hex, b2a_base64, hexlify
-
-                width = height = ''
-                if self.width:
-                    width = ' width="%d"' % self.width
-                if self.height:
-                    height = ' height="%d"' % self.height
-
-                # External URLs and potentially local files are not embedded into the
-                # notebook output.
-                if not self.embed:
-                    url = self.url if self.url is not None else self.filename
-                    output = """<video src="{0}" {1} {2} {3}>
-Your browser does not support the <code>video</code> element.
-</video>""".format(url, self.html_attributes, width, height)
-                    return output
-
-                # Embedded videos are base64-encoded.
-                mimetype = self.mimetype
-                if self.filename is not None:
-                    if not mimetype:
-                        mimetype, _ = mimetypes.guess_type(self.filename)
-
-                    with open(self.filename, 'rb') as f:
-                        video = f.read()
-                else:
-                    video = self.data
-                if isinstance(video, str):
-                    # unicode input is already b64-encoded
-                    b64_video = video
-                else:
-                    b64_video = b2a_base64(video).decode('ascii').rstrip()
-
-                output = """<video {0} {1} {2}>
- <source src="data:{3};base64,{4}" type="{3}">
- Your browser does not support the video tag.
- </video>""".format(self.html_attributes, width, height, mimetype, b64_video)
-                return output
+        # Requires Ipython 7.14 or higher, for this patch: https://github.com/ipython/ipython/pull/12212/
 
         filepath = mkstemp(suffix=".ogv")[1]
         self.save(filepath, nb_loops=1, resolution=resolution, **kwargs)
-        return CustomIPythonVideo(filepath, embed=True, width=resolution[0], html_attributes="controls loop autoplay")
+        return Video(filepath, embed=True, width=resolution[0], html_attributes="controls loop autoplay")
```

### Comparing `capytaine-1.5.post1/capytaine/ui/vtk/body_viewer.py` & `capytaine-2.0/capytaine/ui/vtk/body_viewer.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/ui/vtk/helpers.py` & `capytaine-2.0/capytaine/ui/vtk/helpers.py`

 * *Files identical despite different names*

### Comparing `capytaine-1.5.post1/capytaine/ui/vtk/mesh_viewer.py` & `capytaine-2.0/capytaine/ui/vtk/mesh_viewer.py`

 * *Files identical despite different names*

