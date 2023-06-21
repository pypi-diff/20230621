# Comparing `tmp/Jord-0.0.5.tar.gz` & `tmp/Jord-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jord-0.0.5.tar", last modified: Fri Mar 10 11:30:55 2023, max compression
+gzip compressed data, was "Jord-0.0.6.tar", last modified: Wed Jun 21 08:31:47 2023, max compression
```

## Comparing `Jord-0.0.5.tar` & `Jord-0.0.6.tar`

### file list

```diff
@@ -1,65 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.098493 Jord-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.090493 Jord-0.0.5/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-10 11:30:55.000000 Jord-0.0.5/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-10 11:30:55.000000 Jord-0.0.5/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 11:30:55.000000 Jord-0.0.5/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-10 11:30:55.000000 Jord-0.0.5/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-10 11:30:55.000000 Jord-0.0.5/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-03-10 11:30:50.000000 Jord-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-10 11:30:55.098493 Jord-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-10 11:30:50.000000 Jord-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.090493 Jord-0.0.5/jord/
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.090493 Jord-0.0.5/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/gdal_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/gdal_utilities/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/gdal_utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/gdal_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/gdal_utilities/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/gdal_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/gdal_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.090493 Jord-0.0.5/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/pillow_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/pillow_utilities/exif.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.094493 Jord-0.0.5/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.094493 Jord-0.0.5/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/configuration/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.094493 Jord-0.0.5/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/conversion/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.094493 Jord-0.0.5/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/helpers/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/helpers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.094493 Jord-0.0.5/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/numpy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/numpy_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.094493 Jord-0.0.5/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.098493 Jord-0.0.5/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/shapely_utilities/clamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/shapely_utilities/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/shapely_utilities/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/shapely_utilities/sanitise_poly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.098493 Jord-0.0.5/jord/shapely_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/shapely_utilities/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/shapely_utilities/serialisation/well_known_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-10 11:30:50.000000 Jord-0.0.5/jord/shapely_utilities/serialisation/well_known_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-10 11:30:50.000000 Jord-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-10 11:30:55.098493 Jord-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-03-10 11:30:50.000000 Jord-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:30:55.098493 Jord-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-10 11:30:50.000000 Jord-0.0.5/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-10 11:30:50.000000 Jord-0.0.5/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.485349 Jord-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.457348 Jord-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-21 08:31:41.000000 Jord-0.0.6/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-21 08:31:41.000000 Jord-0.0.6/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 08:31:41.000000 Jord-0.0.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:41.000000 Jord-0.0.6/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.461349 Jord-0.0.6/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-21 08:31:47.000000 Jord-0.0.6/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-21 08:31:47.000000 Jord-0.0.6/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:31:47.000000 Jord-0.0.6/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-21 08:31:47.000000 Jord-0.0.6/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 08:31:47.000000 Jord-0.0.6/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 08:31:41.000000 Jord-0.0.6/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-21 08:31:41.000000 Jord-0.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 08:31:41.000000 Jord-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-21 08:31:47.485349 Jord-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-21 08:31:41.000000 Jord-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 08:31:41.000000 Jord-0.0.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.461349 Jord-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 08:31:41.000000 Jord-0.0.6/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.461349 Jord-0.0.6/jord/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.461349 Jord-0.0.6/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/gdal_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/gdal_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/gdal_utilities/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/gdal_utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/gdal_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/gdal_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/gdal_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.461349 Jord-0.0.6/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/geojson_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/geojson_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.461349 Jord-0.0.6/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/geopandas_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/geopandas_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/geopandas_utilities/geometry_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.465349 Jord-0.0.6/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/pillow_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/pillow_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/pillow_utilities/exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.465349 Jord-0.0.6/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.465349 Jord-0.0.6/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/configuration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/configuration/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.465349 Jord-0.0.6/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/conversion/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.469349 Jord-0.0.6/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/helpers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.469349 Jord-0.0.6/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/numpy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/numpy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/numpy_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/numpy_utilities/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/numpy_utilities/rasters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.473349 Jord-0.0.6/jord/qgis_utilities/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.473349 Jord-0.0.6/jord/qgis_utilities/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.473349 Jord-0.0.6/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qlive_utilities/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qlive_utilities/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qlive_utilities/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.473349 Jord-0.0.6/jord/qt_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qt_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.473349 Jord-0.0.6/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/rasterio_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.477349 Jord-0.0.6/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.477349 Jord-0.0.6/jord/shapely_utilities/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/analysis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/analysis/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/mirroring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/sanitise_poly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.481349 Jord-0.0.6/jord/shapely_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/serialisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/serialisation/well_known_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/shapely_utilities/serialisation/well_known_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.485349 Jord-0.0.6/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/torch_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 08:31:42.000000 Jord-0.0.6/jord/torch_utilities/geodata_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 08:31:42.000000 Jord-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 08:31:42.000000 Jord-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 08:31:47.485349 Jord-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-21 08:31:42.000000 Jord-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.485349 Jord-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:31:47.485349 Jord-0.0.6/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-21 08:31:42.000000 Jord-0.0.6/tests/qgis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-21 08:31:42.000000 Jord-0.0.6/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-21 08:31:42.000000 Jord-0.0.6/tests/test_sanity.py
```

### Comparing `Jord-0.0.5/Jord.egg-info/PKG-INFO` & `Jord-0.0.6/Jord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
@@ -18,22 +18,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
+Provides-Extra: extra
 Provides-Extra: samples
 Provides-Extra: pil
-Provides-Extra: dev
 Provides-Extra: gdal
-Provides-Extra: extra
+Provides-Extra: dev
+Provides-Extra: tests
 Provides-Extra: setup
+Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.0.5 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.0.6 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Natural Language ::
 English Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Provides-Extra: tests Provides-Extra: docs Provides-Extra: samples Provides-
-Extra: pil Provides-Extra: dev Provides-Extra: gdal Provides-Extra: extra
-Provides-Extra: setup Provides-Extra: all License-File: LICENSE.md
+Provides-Extra: extra Provides-Extra: samples Provides-Extra: pil Provides-
+Extra: gdal Provides-Extra: dev Provides-Extra: tests Provides-Extra: setup
+Provides-Extra: docs Provides-Extra: all License-File: LICENSE.md
                                    [header]
                               ****** Jord ******
  | [![Build Status](https://travis-ci.org/aivclab/jord.svg?branch=master)]
 (https://travis-ci.org/aivclab/jord) | [![Coverage Status](https://
 coveralls.io/repos/github/aivclab/vision/badge.svg?branch=master)](https://
 coveralls.io/github/aivclab/vision?branch=master) | [![GitHub Issues](https://
 img.shields.io/github/issues/aivclab/vision.svg?style=flat)](https://
```

### Comparing `Jord-0.0.5/Jord.egg-info/SOURCES.txt` & `Jord-0.0.6/Jord.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,111 @@
+CONTRIBUTING.md
+KEYWORDS.md
 LICENSE.md
+MANIFEST.in
 README.md
+SECURITY.md
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
+.github/CODE_OF_CONDUCT.md
+.github/CONTRIBUTING.md
+.github/PULL_REQUEST_TEMPLATE.md
 Jord.egg-info/PKG-INFO
 Jord.egg-info/SOURCES.txt
 Jord.egg-info/dependency_links.txt
 Jord.egg-info/requires.txt
 Jord.egg-info/top_level.txt
+docs/README.md
+jord/README.md
 jord/__init__.py
+jord/gdal_utilities/README.md
 jord/gdal_utilities/__init__.py
 jord/gdal_utilities/cloning.py
 jord/gdal_utilities/context.py
 jord/gdal_utilities/conversion.py
-jord/gdal_utilities/dataset.py
 jord/gdal_utilities/enums.py
 jord/gdal_utilities/importing.py
+jord/geojson_utilities/README.md
+jord/geojson_utilities/__init__.py
+jord/geojson_utilities/geometry_types.py
+jord/geopandas_utilities/README.md
+jord/geopandas_utilities/__init__.py
+jord/geopandas_utilities/geometry_filtering.py
+jord/pillow_utilities/README.md
 jord/pillow_utilities/__init__.py
 jord/pillow_utilities/exif.py
 jord/pillow_utilities/tiff.py
+jord/qgis_utilities/README.md
 jord/qgis_utilities/__init__.py
+jord/qgis_utilities/categorisation.py
+jord/qgis_utilities/data_provider.py
+jord/qgis_utilities/enums.py
+jord/qgis_utilities/geometry_types.py
 jord/qgis_utilities/importing.py
+jord/qgis_utilities/styling.py
+jord/qgis_utilities/configuration/README.md
 jord/qgis_utilities/configuration/__init__.py
 jord/qgis_utilities/configuration/plugin_settings.py
 jord/qgis_utilities/configuration/project_settings.py
+jord/qgis_utilities/conversion/README.md
 jord/qgis_utilities/conversion/__init__.py
 jord/qgis_utilities/conversion/parsing.py
+jord/qgis_utilities/helpers/README.md
 jord/qgis_utilities/helpers/__init__.py
+jord/qgis_utilities/helpers/actions.py
 jord/qgis_utilities/helpers/drawing.py
 jord/qgis_utilities/helpers/environment.py
 jord/qgis_utilities/helpers/models.py
 jord/qgis_utilities/helpers/progress_bar.py
 jord/qgis_utilities/helpers/sessions.py
 jord/qgis_utilities/helpers/signals.py
 jord/qgis_utilities/helpers/timestamp.py
+jord/qgis_utilities/numpy_utilities/README.md
 jord/qgis_utilities/numpy_utilities/__init__.py
 jord/qgis_utilities/numpy_utilities/conversion.py
+jord/qgis_utilities/numpy_utilities/data_type.py
 jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+jord/qgis_utilities/numpy_utilities/rasters.py
+jord/qgis_utilities/qlive_utilities/README.md
+jord/qgis_utilities/qlive_utilities/__init__.py
+jord/qgis_utilities/qlive_utilities/procedure_implementation.py
+jord/qgis_utilities/qlive_utilities/rpc_protocol.py
+jord/qgis_utilities/shapely_utilities/README.md
+jord/qgis_utilities/shapely_utilities/__init__.py
+jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
+jord/qlive_utilities/README.md
+jord/qlive_utilities/__init__.py
+jord/qlive_utilities/client.py
+jord/qlive_utilities/procedures.py
+jord/qlive_utilities/serialisation.py
+jord/qlive_utilities/uri_utilities.py
+jord/qt_utilities/__init__.py
+jord/qt_utilities/enums.py
+jord/rasterio_utilities/README.md
 jord/rasterio_utilities/__init__.py
+jord/shapely_utilities/README.md
 jord/shapely_utilities/__init__.py
 jord/shapely_utilities/clamp.py
+jord/shapely_utilities/geometry_types.py
+jord/shapely_utilities/iteration.py
 jord/shapely_utilities/lines.py
+jord/shapely_utilities/mirroring.py
 jord/shapely_utilities/morphology.py
+jord/shapely_utilities/points.py
+jord/shapely_utilities/projection.py
 jord/shapely_utilities/sanitise_poly.py
+jord/shapely_utilities/analysis/README.md
+jord/shapely_utilities/analysis/__init__.py
+jord/shapely_utilities/analysis/degrees_of_freedom.py
+jord/shapely_utilities/analysis/tracing.py
+jord/shapely_utilities/serialisation/README.md
 jord/shapely_utilities/serialisation/__init__.py
 jord/shapely_utilities/serialisation/well_known_binary.py
 jord/shapely_utilities/serialisation/well_known_text.py
+jord/torch_utilities/README.md
+jord/torch_utilities/__init__.py
+jord/torch_utilities/geodata_dataset.py
 tests/test_import.py
-tests/test_sanity.py
+tests/test_sanity.py
+tests/qgis/README.md
```

### Comparing `Jord-0.0.5/Jord.egg-info/requires.txt` & `Jord-0.0.6/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 numpy>=1.20.2
 warg
 apppath
 
 [all]
-black[jupyter]>=21.5b0
-apppath
+wheel>=0.33.0
+twine>=1.13.0
+pytest>=4.3.0
+pytest-cov>=2.11.1
+sphinxcontrib-programoutput
+mock
 furo
-pytest>=4.4.1
+sphinx>=4.0.1
+warg
+apppath
+Pillow
 numpy>=1.20.2
 coveralls>=1.6.0
-Pillow
-pytest>=4.3.0
-warg
+pytest>=4.4.1
+pre-commit>=2.17.0
 pip>=22.1.2
+black[jupyter]>=21.5b0
+
+[dev]
+wheel>=0.33.0
 twine>=1.13.0
+pytest>=4.3.0
+pytest-cov>=2.11.1
 sphinxcontrib-programoutput
-wheel>=0.33.0
 mock
+furo
 sphinx>=4.0.1
-pytest-cov>=2.11.1
-pre-commit>=2.17.0
-
-[dev]
-black[jupyter]>=21.5b0
+warg
 apppath
-furo
-pytest>=4.4.1
-mock
 numpy>=1.20.2
-pytest>=4.3.0
-warg
-pip>=22.1.2
-twine>=1.13.0
-wheel>=0.33.0
-sphinxcontrib-programoutput
 coveralls>=1.6.0
-sphinx>=4.0.1
-pytest-cov>=2.11.1
+pytest>=4.4.1
 pre-commit>=2.17.0
+pip>=22.1.2
+black[jupyter]>=21.5b0
 
 [docs]
-sphinx>=4.0.1
 furo
+sphinx>=4.0.1
 sphinxcontrib-programoutput
 
 [extra]
 
 [gdal]
 
 [pil]
 Pillow
 
 [samples]
 
 [setup]
 
 [tests]
-mock
 pytest>=4.4.1
+mock
```

### Comparing `Jord-0.0.5/LICENSE.md` & `Jord-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.5/PKG-INFO` & `Jord-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
@@ -18,22 +18,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
+Provides-Extra: extra
 Provides-Extra: samples
 Provides-Extra: pil
-Provides-Extra: dev
 Provides-Extra: gdal
-Provides-Extra: extra
+Provides-Extra: dev
+Provides-Extra: tests
 Provides-Extra: setup
+Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.0.5 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.0.6 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Natural Language ::
 English Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Provides-Extra: tests Provides-Extra: docs Provides-Extra: samples Provides-
-Extra: pil Provides-Extra: dev Provides-Extra: gdal Provides-Extra: extra
-Provides-Extra: setup Provides-Extra: all License-File: LICENSE.md
+Provides-Extra: extra Provides-Extra: samples Provides-Extra: pil Provides-
+Extra: gdal Provides-Extra: dev Provides-Extra: tests Provides-Extra: setup
+Provides-Extra: docs Provides-Extra: all License-File: LICENSE.md
                                    [header]
                               ****** Jord ******
  | [![Build Status](https://travis-ci.org/aivclab/jord.svg?branch=master)]
 (https://travis-ci.org/aivclab/jord) | [![Coverage Status](https://
 coveralls.io/repos/github/aivclab/vision/badge.svg?branch=master)](https://
 coveralls.io/github/aivclab/vision?branch=master) | [![GitHub Issues](https://
 img.shields.io/github/issues/aivclab/vision.svg?style=flat)](https://
```

### Comparing `Jord-0.0.5/README.md` & `Jord-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.5/jord/__init__.py` & `Jord-0.0.6/jord/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,38 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import datetime
 import os
+from pathlib import Path
+from typing import Any
 from warnings import warn
 
 import pkg_resources
 from apppath import AppPath
+from warg import dist_is_editable
 
 __project__ = "Jord"
 __author__ = "Christian Heider Nielsen"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Nielsen <christian.heider@alexandra.dk>
 
 Created on 27/04/2019
 
 @author: cnheider
 """
 
-from pathlib import Path
-
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 
-# __all__ = ['PROJECT_APP_PATH', 'PROJECT_NAME', 'PROJECT_VERSION', 'get_version']
-
-
-from typing import Any
-
-
-def dist_is_editable(dist: Any) -> bool:
-    """
-    Return True if given Distribution is an editable installation."""
-    import sys
-    from pathlib import Path
-
-    for path_item in sys.path:
-        egg_link = Path(path_item) / f"{dist.project_name}.egg-link"
-        if egg_link.is_file():
-            return True
-    return False
-
-
 PROJECT_NAME = __project__.lower().strip().replace(" ", "_")
 PROJECT_VERSION = __version__
 PROJECT_YEAR = 2018
 PROJECT_AUTHOR = __author__.lower().strip().replace(" ", "_")
 PROJECT_ORGANISATION = "Aivclab"
 PROJECT_APP_PATH = AppPath(app_name=PROJECT_NAME, app_author=PROJECT_AUTHOR)
 PACKAGE_DATA_PATH = Path(pkg_resources.resource_filename(PROJECT_NAME, "data"))
@@ -62,19 +44,17 @@
     DEVELOP = dist_is_editable(distribution)
 else:
     DEVELOP = True
 
 
 def get_version(append_time: Any = DEVELOP) -> str:
     """
+      :param append_time:
 
-    Args:
-      append_time:
-
-    Returns:
+    :rtype: str
 
     """
     version = __version__
     if not version:
         version = os.getenv("VERSION", "0.0.0")
 
     if append_time:
```

### Comparing `Jord-0.0.5/jord/gdal_utilities/cloning.py` & `Jord-0.0.6/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.5/jord/gdal_utilities/context.py` & `Jord-0.0.6/jord/gdal_utilities/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 __doc__ = r"""
 
            Created on 1/16/23
            """
 
 __all__ = ["SilenceGDALSession"]
 
-from .importing import GDAL
 from warg import AlsoDecorator
 
+from .importing import GDAL
+
 
 class SilenceGDALSession(AlsoDecorator):
     """
     Session for silencing gdal warning and errors.
     TODO: add support for having a lasting side effect or leaving last set state of error/exception handling
     """
```

### Comparing `Jord-0.0.5/jord/gdal_utilities/conversion.py` & `Jord-0.0.6/jord/gdal_utilities/conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,37 +76,42 @@
 def copy_gcps_to_file(file: Path, gcps: List[GDAL.GCP]) -> None:
     """
 
     :param file:
     :type file:
     :param gcps:
     :type gcps:
+    :rtype:None
     """
 
     with GDAL.Open(file, GdalAccessEnum.update.value) as f:
         f.SetGCPs(gcps)
         f.FlushCache()
 
 
 def geotiff_to_tiff(src: Path, dst: Path) -> None:
     """
     https://gdal.org/user/translate.html
+
+    :rtype: None
     """
     GDAL.Translate(
         dst,
         src,
         format="JPEG",
         outputType=GDAL.GDT_Byte,
         creationOptions=["COMPRESS=LZW"],
     )
 
 
 def tiff_to_geotiff(src: Path, dst: Path) -> None:
     """
     https://gdal.org/user/translate.html
+
+    :rtype: None
     """
     GDAL.Translate(
         dst,
         src,
         format="GTiff",
         outputType=GDAL.GDT_Byte,
         creationOptions=["COMPRESS=LZW"],
```

### Comparing `Jord-0.0.5/jord/gdal_utilities/importing.py` & `Jord-0.0.6/jord/gdal_utilities/importing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 __author__ = "heider"
 __doc__ = r"""
 
            Created on 5/5/22
            """
 
-__all__ = ["import_gdal", "import_osr", "import_ogr", "GDAL", "OSR", "OGR"]
-
 from types import ModuleType
 
+__all__ = ["import_gdal", "import_osr", "import_ogr", "GDAL", "OSR", "OGR"]
+
 
 def import_gdal() -> ModuleType:
     try:
         import gdal
 
     except (ImportError, ModuleNotFoundError) as e:
         try:
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/configuration/plugin_settings.py` & `Jord-0.0.6/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,19 +13,33 @@
 
 from qgis.core import QgsSettings
 
 from jord import PROJECT_NAME
 
 
 def store_plugin_setting(key: str, value: Any, *, project_name: str = PROJECT_NAME):
+    """
+
+    :param key:
+    :param value:
+    :param project_name:
+    :return:
+    """
     QgsSettings().setValue(f"{project_name}/{key}", value)
 
 
 def read_plugin_setting(
     key: str, *, default_value: Any = None, project_name: str = PROJECT_NAME
 ):
+    """
+
+    :param key:
+    :param default_value:
+    :param project_name:
+    :return:
+    """
     return QgsSettings().value(f"{project_name}/{key}", default_value)
 
 
 if __name__ == "__main__":
     store_plugin_setting("mytext", "hello world")
     print(read_plugin_setting("mytext"))
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/configuration/project_settings.py` & `Jord-0.0.6/jord/qgis_utilities/configuration/project_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,21 +22,34 @@
 
 qgis_project = QgsProject.instance()
 
 
 def restore_default_project_settings(
     defaults: Optional[Mapping] = None, *, project_name: str = PROJECT_NAME
 ):
+    """
+
+    :param defaults:
+    :param project_name:
+    :return:
+    """
     if defaults is None:
         defaults = {}
     for key, value in defaults.items():
         store_project_setting(key, value, project_name=project_name)
 
 
 def store_project_setting(key: str, value: Any, *, project_name: str = PROJECT_NAME):
+    """
+
+    :param key:
+    :param value:
+    :param project_name:
+    :return:
+    """
     if isinstance(value, bool):
         qgis_project.writeEntryBool(project_name, key, value)
     elif isinstance(value, float):
         qgis_project.writeEntryDouble(project_name, key, value)
     # elif isinstance(value, int): # DOES NOT EXIST!
     #    qgis_project.writeEntryNum(project_name, key, value)
     else:
@@ -49,14 +62,23 @@
 def read_project_setting(
     key: str,
     type_hint: type = None,
     *,
     defaults: Mapping = None,
     project_name: str = PROJECT_NAME,
 ):
+    """
+
+    :param key:
+    :param type_hint:
+    :param defaults:
+    :param project_name:
+    :return:
+    """
+
     # read values (returns a tuple with the value, and a status boolean
     # which communicates whether the value retrieved could be converted to
     # its type, in these cases a string, an integer, a double and a boolean
     # respectively)
 
     if defaults is None:
         defaults = {}
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/helpers/drawing.py` & `Jord-0.0.6/jord/qgis_utilities/helpers/drawing.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,18 @@
     Create a rubber band on the canvas.
 
     :param canvas: The canvas to create the rubber band on.
     :return: The rubber band.
     """
     fill_color = QtGui.QColor("white")
     fill_color.setAlphaF(0.0)
+
     stroke_color = QtGui.QColor("red")
     stroke_color.setAlphaF(0.65)
+
     rubber_band = QgsRubberBand(canvas, QgsWkbTypes.PolygonGeometry)
     rubber_band.setWidth(2)
     rubber_band.setColor(fill_color)  # fill color
     rubber_band.setStrokeColor(stroke_color)  # stroke color
     rubber_band.setLineStyle(Qt.DotLine)
+
     return rubber_band
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/helpers/environment.py` & `Jord-0.0.6/jord/qgis_utilities/helpers/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 import cgi
 import subprocess
 from pathlib import Path
 
 __all__ = ["install_requirements_from_file", "install_requirements_from_name"]
 
-from typing import Iterable, Tuple
-
+from typing import Iterable, Tuple, Optional
+import os
 from subprocess import check_output
 import sys
 
 SP_CALLABLE = subprocess.check_call  # subprocess.call
 
 
 def install_requirements_from_file(requirements_path: Path) -> None:
@@ -54,18 +54,18 @@
             return True
     if get_installed_version(requirement_name):
         return True
     return False
 
 
 def requirement_has_version(requirement_name: str) -> bool:
-    return get_requirement_version(requirement_name) != None
+    return get_requirement_version(requirement_name) is not None
 
 
-def get_requirement_version(requirement_name: str) -> str:
+def get_requirement_version(requirement_name: str) -> Optional[str]:
     s = requirement_name.split("==")
     if len(s) == 2:
         return s[-1]
     return None
 
 
 def get_installed_version(requirement_name: str) -> str:
@@ -76,22 +76,29 @@
         if dist:
             return dist.parsed_version  # .version
     except pkg_resources.DistributionNotFound as e:
         pass
     return None
 
 
-def get_newest_version(requirement_name: str) -> str:
+def get_newest_version(
+    requirement_name: str,
+    pip_index=os.environ.get("PIP_INDEX_URL", "https://pypi.org/pypi/"),
+) -> str:
+    """
+
+    :param requirement_name:
+    :param pip_index:
+    :return:
+    """
     from pkg_resources import parse_version
-    import os
+
     import json
     from urllib.request import Request, urlopen
 
-    DEFAULT_PIP_INDEX = os.environ.get("PIP_INDEX_URL", "https://pypi.org/pypi/")
-
     def get_charset(headers, default: str = "utf-8"):
         # this is annoying.
         try:
             charset = headers.get_content_charset(default)
         except AttributeError:
             # Python 2
             charset = headers.getparam("charset")
@@ -111,20 +118,20 @@
             raise err
         raw_data = response.read()
         response_encoding = get_charset(response.headers)
         decoded_data = raw_data.decode(response_encoding)
         data = json.loads(decoded_data)
         return data
 
-    def get_data_pypi(name: str, index: str = DEFAULT_PIP_INDEX):
+    def get_data_pypi(name: str, index: str = pip_index):
         uri = f"{index.rstrip('/')}/{name.split('[')[0]}/json"
         data = json_get(uri)
         return data
 
-    def get_versions_pypi(name: str, index: str = DEFAULT_PIP_INDEX):
+    def get_versions_pypi(name: str, index: str = pip_index):
         data = get_data_pypi(name, index)
         version_numbers = sorted(data["releases"], key=parse_version)
         return tuple(version_numbers)
 
     return parse_version(get_versions_pypi(requirement_name)[-1])
 
 
@@ -167,21 +174,25 @@
         SP_CALLABLE(["pip"] + args)
     # subprocess.check_call([sys.executable, '-m', 'conda', 'install', '<packagename>'])
     elif True:
         interpreter = Path(sys.executable).absolute()
         SP_CALLABLE([str(interpreter), "-m", "pip"] + args)
 
 
-def remove_requirements_from_name(*requirements_name: Iterable[str]) -> None:
+def remove_requirements_from_name(
+    *requirements_name: Iterable[str], num_repeat: int = 1
+) -> None:
     """
-
     Multiple colliding versions may be installed at once, (conda, pip, ....)
-    Repeat args let you choose how many time to try uninstall the packages.
+
+    :param num_repeat:     Repeat arg let you choose how many times to try to uninstall the packages.
+    :param requirements_name:
+    :return:
     """
-    num_repeat: int = 1
+
     args = ["uninstall", "-y", *requirements_name]
 
     for _ in range(num_repeat):
         if False:
             import pip
 
             pip.main(args)
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/helpers/models.py` & `Jord-0.0.6/jord/qgis_utilities/helpers/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Any, Optional, Tuple
 
 from qgis.PyQt import QtCore
 
 __all__ = ["MyTableModel"]
 
 
+# noinspection PyPep8Naming
 class MyTableModel(QtCore.QAbstractTableModel):
     """
     A model that can be used to display a table of data.
 
     :param data: The data to display.
     :param parent: The parent object.
 
@@ -25,29 +26,29 @@
 
     def __init__(self, data: Tuple = (()), parent: Any = None):
         super().__init__(parent)
         self.data = data
 
     def headerData(
         self, section: int, orientation: QtCore.Qt.Orientation, role: int
-    ) -> str:
+    ) -> str:  # Do not rename
         """
 
         :param section:
         :param orientation:
         :param role:
         :return:
         """
         if role == QtCore.Qt.DisplayRole:
             if orientation == QtCore.Qt.Horizontal:
                 return f"Column {str(section)}"
             else:
                 return f"Row {str(section)}"
 
-    def columnCount(self, parent: Any = None) -> int:
+    def columnCount(self, parent: Any = None) -> int:  # Do not rename
         """
 
         :param parent:
         :return:
         """
         if self.rowCount():
             return len(self.data[0])
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/helpers/progress_bar.py` & `Jord-0.0.6/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,23 @@
     :type minimum_width: int
     :return: The dialog.
     :rtype: Tuple[QtWidgets.QDialog, QtWidgets.QProgressBar]
     """
     dialog = QtGui.QProgressDialog()
     dialog.setWindowTitle("Progress")
     dialog.setLabelText("text")
+
     bar = QtWidgets.QProgressBar(dialog)
     bar.setTextVisible(True)
     bar.setValue(progress)
+
     dialog.setBar(bar)
     dialog.setMinimumWidth(minimum_width)
     dialog.show()
+
     return dialog, bar
 
 
 if __name__ == "__main__":
 
     def calc(x, y):
         from time import sleep
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/helpers/signals.py` & `Jord-0.0.6/jord/qgis_utilities/helpers/signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def connect_signal(signal: QtCore.pyqtSignal, new_handler: callable = None) -> None:
     """
 
     :param signal:
     :param new_handler:
     :return:
     """
-    if new_handler is not None:  # if newhandler is not None, connect it
+    if new_handler is not None:  # if new_handler is not None, connect it
         signal.connect(new_handler)
     else:
         if IS_DEBUGGING:
             raise Exception("new_handler is None")
         warning("new_handler is None")
 
 
@@ -36,15 +36,15 @@
 
     :param signal:
     :param old_handler:
     :return:
     """
     if signal is not None:
         try:
-            if old_handler is not None:  # disconnect oldhandler(s)
+            if old_handler is not None:  # disconnect old_handler(s)
                 while True:
                     # the loop is needed for safely disconnecting a specific handler,
                     # because it may have been connected multple times,
                     # and disconnect(slot) only removes one connection at a time.
                     signal.disconnect(old_handler)
             else:  # disconnect all, only available when old_handler is None and we are debugging, as this is bad practice
                 if IS_DEBUGGING:
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/helpers/timestamp.py` & `Jord-0.0.6/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.5/jord/qgis_utilities/numpy_utilities/conversion.py` & `Jord-0.0.6/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,20 @@
     "get_qimage_from_numpy",
     "transform_coordinates",
     "get_coordinates_of_layer_extent",
 ]
 
 
 def get_qimage_from_numpy(img: Image, debug: bool = False) -> QtGui.QImage:
+    """
+
+    :param img:
+    :param debug:
+    :return:
+    """
     # if isinstance(img, Image):
     #    img = img.data
     # if isinstance(img, numpy.ndarray):
     #    img = img.data
 
     # if isinstance(img, cv2.Image):
     #    img = img.data # QtGui.QImage.Format_BGR888
@@ -47,15 +53,21 @@
 
     return QtGui.QImage(img, width, height, bytes_per_line, QtGui.QImage.Format_RGB888)
 
 
 def transform_coordinates(coordinates: Sequence, from_crs: str, to_crs: str) -> list:
     """
 
-    function to transform a set of coordinates from one CRS to another"""
+    function to transform a set of coordinates from one CRS to another
+
+
+    :param coordinates:
+    :param from_crs:
+    :param to_crs:
+    :return:"""
     crs_src = QgsCoordinateReferenceSystem(from_crs)
     crs_dest = QgsCoordinateReferenceSystem(to_crs)
     xform = QgsCoordinateTransform(crs_src, crs_dest)
 
     coordinates_as_points = [
         QgsPoint(coordinates[0], coordinates[1]),
         QgsPoint(coordinates[2], coordinates[3]),
@@ -74,14 +86,18 @@
 
 
 def get_coordinates_of_layer_extent(layer: QgsVectorLayer) -> list:
     """
 
     function to get coordinates of a layer extent
 
+
+    :param layer:
+    :return:
+
     """
 
     layerRectangle = layer.extent()
 
     return [
         layerRectangle.xMinimum(),
         layerRectangle.yMinimum(),
```

### Comparing `Jord-0.0.5/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `Jord-0.0.6/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 02-12-2020
            """
 
+import numpy
 from qgis.PyQt import QtGui
 from qgis.PyQt.QtCore import QEvent, Qt
 from qgis.gui import QgsPixmapLabel
-
+from typing import Any
 from .conversion import get_qimage_from_numpy
 
 __all__ = ["NumpyImageWidget"]
 
 
 class NumpyImageWidget(QgsPixmapLabel):
     """solely for the purpose of the maintaining the aspect ratio of the image"""
 
-    def __init__(self, parent=None):
+    def __init__(self, parent: Any = None):
         super().__init__(parent)
         # self.setScaledContents(True)
         # self.setSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         # self.setSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Minimum)
         # self.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         # self.setSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Maximum)
         # self.setSizePolicy(QtWidgets.QSizePolicy.Ignored, QtWidgets.QSizePolicy.Ignored)
@@ -32,15 +33,19 @@
         self.setText("Waiting for layer...")
         self.setToolTip("Waiting for layer...")
         # self.setCentralWidget(self.label)
         # self.label.adjustSize()
         # self.resize(self.pixmap.width(), self.pixmap.height())
         # self.installEventFilter(self)
 
-    def recalculate_size(self):  # TODO: maybe reset to non scaled img
+    def recalculate_size(self) -> None:  # TODO: maybe reset to non scaled img
+        """
+
+        :return:
+        """
         if False:
             self.pixmap = self.pixmap.scaled(
                 self.size(), Qt.KeepAspectRatio, transformMode=Qt.SmoothTransformation
             )
         elif False:  #
             self.pixmap = self.pixmap.scaledToWidth(
                 self.width(), mode=Qt.SmoothTransformation
@@ -54,19 +59,30 @@
 
         # self.setMinimumSize(img.shape[1], img.shape[0])
         # self.setMinimumSize(pixmap.width(), pixmap.height())
         # self.setMinimumSize(1,1)
 
         self.setPixmap(self.pixmap)
 
-    def setImage(self, img):
+    def setImage(self, img: numpy.ndarray) -> None:
+        """
+
+        :param img:
+        :return:
+        """
         self.pixmap = QtGui.QPixmap.fromImage(get_qimage_from_numpy(img))
         self.recalculate_size()
 
-    def eventFilter(self, source, event):
+    def eventFilter(self, source: Any, event: Any) -> Any:
+        """
+
+        :param source:
+        :param event:
+        :return:
+        """
         if source is self and event.type() == QEvent.Resize:
             # print("resize")
             if False:
                 if self.pixmap():
                     self.recalculate_size()
         return super().eventFilter(source, event)
```

### Comparing `Jord-0.0.5/jord/shapely_utilities/clamp.py` & `Jord-0.0.6/jord/shapely_utilities/clamp.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,45 +5,61 @@
 __doc__ = r"""
 
            Created on 1/23/23
            """
 
 __all__ = [
     "split_line_string",
-    "unsplit_line_string",
+    "combine_line_string",
     "extend_segment",
     "fix_starting_point",
     "adjust_line_end",
     "ensure_list_of_geometries",
 ]
 
 from collections import deque
 from typing import List, Sequence, Union
 
-from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 from shapely.geometry import LineString, MultiLineString, Point, Polygon
+from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 
 
 def split_line_string(line_string: LineString) -> Sequence[LineString]:
-    """Break a LineString"""
+    """
+    Break a LineString
+
+    :param line_string:
+    :return:
+    """
     for start, end in zip(line_string.coords[:-1], line_string.coords[1:]):
         yield LineString((start, end))
 
 
-def unsplit_line_string(segments: Sequence[LineString]) -> LineString:
+def combine_line_string(segments: Sequence[LineString]) -> LineString:
+    """
+
+    :param segments:
+    :return:
+    :rtype: LineString
+    """
     coords = [segments[0].coords[0]]
 
     for segment in segments:
         coords.extend(segment.coords[1:])
 
     return LineString(coords)
 
 
 def extend_segment(line_string: LineString) -> LineString:
-    """Move a line segment's start and end away from each other to ensure intersections."""
+    """
+    Move a line segment's start and end away from each other to ensure intersections
+
+    :param line_string:
+    :return:
+    """
     p0 = line_string.coords[0]
     p1 = line_string.coords[1]
 
     difference = (p0[0] - p1[0], p0[1] - p1[1])
     length = (difference[0] ** 2 + difference[1] ** 2) ** 0.5
     direction = (difference[0] / length, difference[1] / length)
     offset = (direction[0] * 1e-12, direction[1] * 1e-12)
@@ -51,22 +67,27 @@
     new_p0 = (p0[0] + offset[0], p0[1] + offset[1])
     new_p1 = (p1[0] - offset[0], p1[1] - offset[1])
 
     return LineString((new_p0, new_p1))
 
 
 def fix_starting_point(polygon_pieces: Sequence[Polygon]) -> Sequence[Polygon]:
-    """Reconnect the starting point of a polygon's pieces.
+    """
+    Reconnect the starting point of a polygon's pieces.
     When splitting a polygon with two lines, we want to get two pieces.
     However, that's not quite how Shapely works.  The outline of the
     polygon is a LinearRing that starts and ends at the same place, but
     Shapely still knows where that starting point is and splits there
     too.
     We don't want that third piece, so we'll reconnect the segments that
     touch the starting point.
+
+
+    :param polygon_pieces:
+    :return:
     """
 
     if len(polygon_pieces) == 3:
         # Fortunately, Shapely keeps the starting point of the LinearRing
         # as the starting point of the first segment.  That means it's also
         # the ending point of the last segment.  Reconnecting is super simple:
         return [
@@ -74,41 +95,58 @@
             LineString(polygon_pieces[2].coords[:] + polygon_pieces[0].coords[1:]),
         ]
     else:
         return polygon_pieces  # We probably cut exactly at the starting point.
 
 
 def adjust_line_end(line: LineString, end: BaseGeometry) -> LineString:
-    """Reverse line if necessary to ensure that it ends near end."""
+    """
+    Reverse line if necessary to ensure that it ends near end.
+
+    :param line:
+    :param end:
+    :return:
+    """
 
     line_start = Point(*line.coords[0])
     line_end = Point(*line.coords[-1])
 
     if line_end.distance(end) < line_start.distance(end):
         return line
     else:
         return LineString(line.coords[::-1])
 
 
 def ensure_list_of_geometries(
     thing: Union[BaseGeometry, BaseMultipartGeometry]
 ) -> List[BaseGeometry]:
+    """
+
+    :param thing:
+    :return:
+    """
     if False:
         try:  # Not MultiGeometry base class for shapely
             return list(thing.geoms)
         except AttributeError:
             return [thing]
     if isinstance(thing, BaseMultipartGeometry):
         return list(thing.geoms)
     return [thing]
 
 
 def clamp_linestring_to_polygon(
     line_string: LineString, polygon: Polygon
 ) -> LineString:
+    """
+
+    :param line_string:
+    :param polygon:
+    :return:
+    """
     segments = deque(split_line_string(line_string))
     result = []
     exiting_segment = None
     was_inside = False
 
     # contains() checks can fail without this.
     buffered_polygon = polygon.buffer(1e-9)
@@ -195,21 +233,21 @@
             # push it and the rest to be reprocessed in the following iterations.
 
             segments.appendleft(
                 LineString((pieces[0].coords[1], current_segment.coords[-1]))
             )
             segments.appendleft(pieces[0])
 
-    return unsplit_line_string(result)
+    return combine_line_string(result)
 
 
 if __name__ == "__main__":
 
     def _main():
-        from draugr.numpy_utilities.space_filling import HilbertCurve
+        from draugr.numpy_utilities import HilbertCurve
         from geopandas import GeoSeries
         from matplotlib import pyplot
 
         hilbert_curve = HilbertCurve(5, 2)
         hc = LineString(hilbert_curve.points_from_distances(range(1023)))
         circle = Point(15, 15).buffer(15)
         clamped = clamp_linestring_to_polygon(hc, circle)
```

### Comparing `Jord-0.0.5/jord/shapely_utilities/morphology.py` & `Jord-0.0.6/jord/shapely_utilities/morphology.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,68 @@
 from shapely.geometry.base import BaseGeometry
 
 __all__ = ["closing", "opening", "erode", "erosion", "dilate", "dilation", "close"]
 
 
 def erosion(geom: BaseGeometry, eps: float = 1e-7) -> BaseGeometry:
+    """
+
+    :param geom: The geometry to be eroded
+    :param eps: Erosion amount
+    :return: The eroded geometry
+    """
     return geom.buffer(-eps)
 
 
 erode = erosion
 
 
 def dilation(geom: BaseGeometry, eps: float = 1e-7) -> BaseGeometry:
+    """
+
+    :param geom: The geometry to be dilated
+    :param eps: Dilation amount
+    :return: The dilated geometry
+    """
     return geom.buffer(eps)
 
 
 dilate = dilation
 
 
 def closing(geom: BaseGeometry, eps: float = 1e-7) -> BaseGeometry:
+    """
+
+    :param geom: The geometry to be closed
+    :param eps: Dilation and Erosion amount
+    :return: The closed geometry
+    """
     return erode(dilate(geom, eps), eps)
 
 
 close = closing
 
 
 def opening(geom: BaseGeometry, eps: float = 1e-7) -> BaseGeometry:
+    """
+
+    :param geom: The geometry to be opened
+    :param eps: Erosion and Dilation amount
+    :return: The opened geometry
+    """
     return dilate(erode(geom, eps), eps)
 
 
 # open = opening # keyword clash
 
 if __name__ == "__main__":
 
     def aishdjauisd():
         # Import constructors for creating geometry collections
-        from shapely.geometry import MultiPoint, MultiLineString, MultiPolygon
+        from shapely.geometry import MultiPoint, MultiLineString
 
         # Import necessary geometric objects from shapely module
         from shapely.geometry import Point, LineString, Polygon
 
         # Create Point geometric object(s) with coordinates
         point1 = Point(2.2, 4.2)
         point2 = Point(7.2, -25.1)
@@ -55,22 +79,22 @@
         line1 = LineString([point1, point2])
         line2 = LineString([point2, point3])
         multi_line = MultiLineString([line1, line2])
         polygon = Polygon([point2, point1, point3])
 
         from shapely.geometry import GeometryCollection
         from matplotlib import pyplot
-        import geopandas as gpd
+        import geopandas
 
         geoms = GeometryCollection([multi_point, multi_point2, multi_line, polygon])
 
         # A positive distance produces a dilation, a negative distance an erosion. A very small or zero distance may sometimes be used to “tidy” a polygon.
         geoms = opening(geoms)
         geoms = dilate(geoms)
         geoms = closing(geoms)
         geoms = erode(geoms)
 
-        p = gpd.GeoSeries(geoms)
+        p = geopandas.GeoSeries(geoms)
         p.plot()
         pyplot.show()
 
     aishdjauisd()
```

### Comparing `Jord-0.0.5/jord/shapely_utilities/serialisation/well_known_text.py` & `Jord-0.0.6/jord/shapely_utilities/serialisation/well_known_text.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,31 @@
+from enum import Enum
 from pathlib import Path
 from typing import Sequence
+
 import pandas
-from shapely import wkt
 from pandas import DataFrame
+from shapely import wkt
 
 __all__ = ["load_wkts_from_csv", "csv_wkt_generator"]
 
+from sorcery import assigned_names
+
+
+class WktTypeEnum(Enum):
+    (
+        point,
+        multipoint,
+        linestring,
+        multilinestring,
+        polygon,
+        multipolygon,
+        geometrycollection,
+    ) = assigned_names()
+
 
 def load_wkts_from_csv(
     csv_file_path: Path, geometry_column: str = "Shape", additional_cols: Sequence = ()
 ) -> DataFrame:
     """
     Well-Known Text
     """
@@ -17,11 +33,26 @@
         str(csv_file_path), usecols=[*additional_cols, geometry_column]
     )
     df[geometry_column] = df[geometry_column].apply(wkt.loads)
     return df
 
 
 def csv_wkt_generator(csv_file_path: Path, geometry_column: str = "Shape") -> wkt:
+    """
+
+    :param csv_file_path:
+    :param geometry_column:
+    :return:
+    """
     for idx, g in pandas.read_csv(
         str(csv_file_path), usecols=[geometry_column]
     ).iterrows():
         yield wkt.loads(g)
+
+
+if __name__ == "__main__":
+
+    def uashdu():
+        for t in WktTypeEnum:
+            print(t)
+
+    uashdu()
```

### Comparing `Jord-0.0.5/setup.py` & `Jord-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 import re
 from pathlib import Path
 from typing import List, Sequence, Union
 
 from setuptools import find_packages, setup
 
 
-def python_version_check(major: int = 3, minor: int = 7):
+def python_version_check(major: int = 3, minor: int = 7) -> None:
     """
-
-    Args:
-      major:
-      minor:
+      :param major:
+    :param minor:
     """
     import sys
 
     assert sys.version_info.major == major and sys.version_info.minor >= minor, (
         f"This project is utilises language features only present Python {major}.{minor} and greater. "
         f"You are running {sys.version_info}."
     )
@@ -73,14 +71,15 @@
 
 with open(Path(__file__).parent / "jord" / "__init__.py", "r") as project_init_file:
     str_reg_exp = "['\"]([^'\"]*)['\"]"
     content = project_init_file.read()  # get strings from module
     version = re.search(rf"__version__ = {str_reg_exp}", content, re.M).group(1)
     project_name = re.search(rf"__project__ = {str_reg_exp}", content, re.M).group(1)
     author = re.search(rf"__author__ = {str_reg_exp}", content, re.M).group(1)
+
 __author__ = author
 
 
 class JordPackage:
     """description"""
 
     @property
@@ -89,15 +88,15 @@
             "requirements_tests.txt", Path(__file__).parent / "requirements"
         )
 
     @property
     def setup_dependencies(self) -> list:
         """
 
-        Returns:
+        :return: requirements
 
         """
         return read_reqs(
             "requirements_setup.txt", Path(__file__).parent / "requirements"
         )
 
     @property
```

