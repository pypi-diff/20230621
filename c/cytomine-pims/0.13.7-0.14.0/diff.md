# Comparing `tmp/cytomine-pims-0.13.7.tar.gz` & `tmp/cytomine-pims-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytomine-pims-0.13.7.tar", last modified: Mon Jun 19 11:04:09 2023, max compression
+gzip compressed data, was "cytomine-pims-0.14.0.tar", last modified: Wed Jun 21 12:09:54 2023, max compression
```

## Comparing `cytomine-pims-0.13.7.tar` & `cytomine-pims-0.14.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.069931 cytomine-pims-0.13.7/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9557 2023-06-19 11:04:09.069931 cytomine-pims-0.13.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     8864 2023-06-09 11:11:39.000000 cytomine-pims-0.13.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.053931 cytomine-pims-0.13.7/cytomine_pims.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9557 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3258 2023-06-19 11:04:09.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.053931 cytomine-pims-0.13.7/pims/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/pims/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.057931 cytomine-pims-0.13.7/pims/api/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10138 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     3620 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/colormaps.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2568 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     3378 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/formats.py
--rw-rw-rw-   0 root         (0) root         (0)    13741 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/histograms.py
--rw-rw-rw-   0 root         (0) root         (0)     4252 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/housekeeping.py
--rw-rw-rw-   0 root         (0) root         (0)    25845 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     8603 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/operations.py
--rw-rw-rw-   0 root         (0) root         (0)     8083 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/resized.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/server.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/spectral.py
--rw-rw-rw-   0 root         (0) root         (0)     7411 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/thumb.py
--rw-rw-rw-   0 root         (0) root         (0)    17122 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/tile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.057931 cytomine-pims-0.13.7/pims/api/utils/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/annotation_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     2713 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/cytomine_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/header.py
--rw-rw-rw-   0 root         (0) root         (0)     6268 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/input_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/mimetype.py
--rw-rw-rw-   0 root         (0) root         (0)    23846 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/models.py
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/output_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     2851 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/parameter.py
--rw-rw-rw-   0 root         (0) root         (0)    10058 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/processing_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     2086 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/range_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     4761 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/response.py
--rw-rw-rw-   0 root         (0) root         (0)     9635 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/window.py
--rw-rw-rw-   0 root         (0) root         (0)     5452 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.057931 cytomine-pims-0.13.7/pims/cache/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/cache/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/cache/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/cache/object.py
--rw-rw-rw-   0 root         (0) root         (0)    11634 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/cache/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     2226 2023-06-06 14:49:46.000000 cytomine-pims-0.13.7/pims/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/docs.py
--rw-rw-rw-   0 root         (0) root         (0)     9417 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/fastapi_tweaks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/files/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5828 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/archive.py
--rw-rw-rw-   0 root         (0) root         (0)    12123 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/file.py
--rw-rw-rw-   0 root         (0) root         (0)     3079 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/histogram.py
--rw-rw-rw-   0 root         (0) root         (0)    17470 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/filters/
--rw-rw-rw-   0 root         (0) root         (0)     6374 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/filters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3796 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/filters/global_histogram.py
--rw-rw-rw-   0 root         (0) root         (0)     8819 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/filters/pixel_color_deconvolution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/formats/
--rw-rw-rw-   0 root         (0) root         (0)     5552 2023-06-08 09:07:51.000000 cytomine-pims-0.13.7/pims/formats/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/formats/common/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3404 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/bmp.py
--rw-rw-rw-   0 root         (0) root         (0)    13688 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/dicom.py
--rw-rw-rw-   0 root         (0) root         (0)     8303 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/imagej.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/jpeg.py
--rw-rw-rw-   0 root         (0) root         (0)     5544 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/jpeg2000.py
--rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/ometiff.py
--rw-rw-rw-   0 root         (0) root         (0)     4928 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/png.py
--rw-rw-rw-   0 root         (0) root         (0)     3648 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/ppm.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/sis.py
--rw-rw-rw-   0 root         (0) root         (0)     5525 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/tiff.py
--rw-rw-rw-   0 root         (0) root         (0)    10568 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/virtual.py
--rw-rw-rw-   0 root         (0) root         (0)     4693 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/webp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/formats/utils/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9505 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/checker.py
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/convertor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/formats/utils/engines/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2707 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/exiftool.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/omexml.py
--rw-rw-rw-   0 root         (0) root         (0)     7698 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/pil.py
--rw-rw-rw-   0 root         (0) root         (0)     7958 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/tifffile.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/vips.py
--rw-rw-rw-   0 root         (0) root         (0)     3405 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     6661 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/histogram.py
--rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10320 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/formats/utils/structures/
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)    13176 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2861 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/planes.py
--rw-rw-rw-   0 root         (0) root         (0)     7924 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/pyramid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/importer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 11:03:58.000000 cytomine-pims-0.13.7/pims/importer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2560 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/importer/import_local_images.py
--rw-rw-rw-   0 root         (0) root         (0)    19599 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/importer/importer.py
--rw-rw-rw-   0 root         (0) root         (0)    24279 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/importer/listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     1953 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/processing/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)     9001 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/colormaps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/processing/histograms/
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/histograms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/histograms/format.py
--rw-rw-rw-   0 root         (0) root         (0)     7616 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/histograms/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    25411 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/image_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5183 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/masks.py
--rw-rw-rw-   0 root         (0) root         (0)    15529 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/pixels.py
--rw-rw-rw-   0 root         (0) root         (0)     6302 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/region.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4746 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/tasks/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/tasks/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.069931 cytomine-pims-0.13.7/pims/utils/
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/arrays.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/background_task.py
--rw-rw-rw-   0 root         (0) root         (0)     6351 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/color.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)     2554 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/copy.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/dict.py
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/dtypes.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/iterables.py
--rw-rw-rw-   0 root         (0) root         (0)     1824 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/math.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/strings.py
--rw-rw-rw-   0 root         (0) root         (0)     2982 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/types.py
--rw-rw-rw-   0 root         (0) root         (0)     2949 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/vips.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-19 11:04:09.069931 cytomine-pims-0.13.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5015 2023-05-23 07:23:23.000000 cytomine-pims-0.13.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.823525 cytomine-pims-0.14.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9557 2023-06-21 12:09:54.823525 cytomine-pims-0.14.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     8864 2023-06-09 11:11:39.000000 cytomine-pims-0.14.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.811525 cytomine-pims-0.14.0/cytomine_pims.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9557 2023-06-21 12:09:54.000000 cytomine-pims-0.14.0/cytomine_pims.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-06-21 12:09:54.000000 cytomine-pims-0.14.0/cytomine_pims.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 12:09:54.000000 cytomine-pims-0.14.0/cytomine_pims.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-21 12:09:54.000000 cytomine-pims-0.14.0/cytomine_pims.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-21 12:09:54.000000 cytomine-pims-0.14.0/cytomine_pims.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.811525 cytomine-pims-0.14.0/pims/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-06-21 12:09:51.000000 cytomine-pims-0.14.0/pims/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.815525 cytomine-pims-0.14.0/pims/api/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10138 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3620 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/colormaps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2568 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/formats.py
+-rw-rw-rw-   0 root         (0) root         (0)    13741 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/histograms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4252 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/housekeeping.py
+-rw-rw-rw-   0 root         (0) root         (0)    25845 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     8603 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     8083 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/resized.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/server.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/spectral.py
+-rw-rw-rw-   0 root         (0) root         (0)     7411 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/thumb.py
+-rw-rw-rw-   0 root         (0) root         (0)    17122 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/tile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.815525 cytomine-pims-0.14.0/pims/api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/annotation_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2713 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/cytomine_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     6268 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/input_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/mimetype.py
+-rw-rw-rw-   0 root         (0) root         (0)    23846 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/output_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2851 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10058 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/processing_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/range_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4761 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/utils/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     9635 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/api/window.py
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.815525 cytomine-pims-0.14.0/pims/cache/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/cache/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/cache/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/cache/object.py
+-rw-rw-rw-   0 root         (0) root         (0)    11634 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/cache/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     2226 2023-06-06 14:49:46.000000 cytomine-pims-0.14.0/pims/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9417 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/fastapi_tweaks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.815525 cytomine-pims-0.14.0/pims/files/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/files/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)    12123 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/files/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/files/histogram.py
+-rw-rw-rw-   0 root         (0) root         (0)    17470 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/files/image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.815525 cytomine-pims-0.14.0/pims/filters/
+-rw-rw-rw-   0 root         (0) root         (0)     6374 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/filters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/filters/global_histogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     8819 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/filters/pixel_color_deconvolution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.815525 cytomine-pims-0.14.0/pims/formats/
+-rw-rw-rw-   0 root         (0) root         (0)     5552 2023-06-08 09:07:51.000000 cytomine-pims-0.14.0/pims/formats/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.819525 cytomine-pims-0.14.0/pims/formats/common/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3404 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/bmp.py
+-rw-rw-rw-   0 root         (0) root         (0)    13688 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/dicom.py
+-rw-rw-rw-   0 root         (0) root         (0)     8303 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/imagej.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/jpeg.py
+-rw-rw-rw-   0 root         (0) root         (0)     5544 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/jpeg2000.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/ometiff.py
+-rw-rw-rw-   0 root         (0) root         (0)     4928 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/png.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/ppm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/sis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5525 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/tiff.py
+-rw-rw-rw-   0 root         (0) root         (0)    10568 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/virtual.py
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/common/webp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.819525 cytomine-pims-0.14.0/pims/formats/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9505 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/convertor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.819525 cytomine-pims-0.14.0/pims/formats/utils/engines/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/engines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/engines/exiftool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/engines/omexml.py
+-rw-rw-rw-   0 root         (0) root         (0)     7698 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/engines/pil.py
+-rw-rw-rw-   0 root         (0) root         (0)     7958 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/engines/tifffile.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/engines/vips.py
+-rw-rw-rw-   0 root         (0) root         (0)     3405 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/histogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10320 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.819525 cytomine-pims-0.14.0/pims/formats/utils/structures/
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/structures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/structures/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13176 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/structures/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2861 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/structures/planes.py
+-rw-rw-rw-   0 root         (0) root         (0)     7924 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/formats/utils/structures/pyramid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.823525 cytomine-pims-0.14.0/pims/importer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 12:09:48.000000 cytomine-pims-0.14.0/pims/importer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/importer/import_local_images.py
+-rw-rw-rw-   0 root         (0) root         (0)    19599 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/importer/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)    24279 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/importer/listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.823525 cytomine-pims-0.14.0/pims/processing/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)     9001 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/colormaps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.823525 cytomine-pims-0.14.0/pims/processing/histograms/
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/histograms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/histograms/format.py
+-rw-rw-rw-   0 root         (0) root         (0)     7616 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/histograms/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    25411 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/image_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     5183 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/masks.py
+-rw-rw-rw-   0 root         (0) root         (0)    15529 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/pixels.py
+-rw-rw-rw-   0 root         (0) root         (0)     6302 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/processing/region.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.823525 cytomine-pims-0.14.0/pims/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/tasks/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/tasks/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:09:54.823525 cytomine-pims-0.14.0/pims/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/arrays.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/background_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/color.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)     2554 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/copy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/dtypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/iterables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/math.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/strings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2982 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-05-09 08:02:09.000000 cytomine-pims-0.14.0/pims/utils/vips.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-21 12:09:54.827525 cytomine-pims-0.14.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5015 2023-05-23 07:23:23.000000 cytomine-pims-0.14.0/setup.py
```

### Comparing `cytomine-pims-0.13.7/LICENSE` & `cytomine-pims-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/PKG-INFO` & `cytomine-pims-0.14.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytomine-pims
-Version: 0.13.7
+Version: 0.14.0
 Summary: Cytomine Python Image Server
 Home-page: https://doc.uliege.cytomine.org
 Author: Ulysse Rubens
 Author-email: uliege@cytomine.org
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cytomine-pims-0.13.7/README.md` & `cytomine-pims-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/cytomine_pims.egg-info/PKG-INFO` & `cytomine-pims-0.14.0/cytomine_pims.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytomine-pims
-Version: 0.13.7
+Version: 0.14.0
 Summary: Cytomine Python Image Server
 Home-page: https://doc.uliege.cytomine.org
 Author: Ulysse Rubens
 Author-email: uliege@cytomine.org
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cytomine-pims-0.13.7/cytomine_pims.egg-info/SOURCES.txt` & `cytomine-pims-0.14.0/cytomine_pims.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/cytomine_pims.egg-info/requires.txt` & `cytomine-pims-0.14.0/cytomine_pims.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/__init__.py` & `cytomine-pims-0.14.0/pims/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/__version__.py` & `cytomine-pims-0.14.0/pims/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 # KEEP ENCODING - so that __version__ can be read even if py2.7 is used.
 
 
 
 __title__ = 'pims'
 __description__ = 'Cytomine Python Image Server'
 __url__ = 'https://doc.uliege.cytomine.org'
-__version__ = "0.13.7"
+__version__ = "0.14.0"
 __api_version__ = "0.0.0"
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2020-2021 ULiège Cytomine R&D team'
 __author__ = 'Ulysse Rubens'
 __email__ = 'uliege@cytomine.org'
```

### Comparing `cytomine-pims-0.13.7/pims/api/__init__.py` & `cytomine-pims-0.14.0/pims/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/annotation.py` & `cytomine-pims-0.14.0/pims/api/annotation.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/colormaps.py` & `cytomine-pims-0.14.0/pims/api/colormaps.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/exceptions.py` & `cytomine-pims-0.14.0/pims/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/filters.py` & `cytomine-pims-0.14.0/pims/api/filters.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/formats.py` & `cytomine-pims-0.14.0/pims/api/formats.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/histograms.py` & `cytomine-pims-0.14.0/pims/api/histograms.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/housekeeping.py` & `cytomine-pims-0.14.0/pims/api/housekeeping.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/metadata.py` & `cytomine-pims-0.14.0/pims/api/metadata.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/operations.py` & `cytomine-pims-0.14.0/pims/api/operations.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/resized.py` & `cytomine-pims-0.14.0/pims/api/resized.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/server.py` & `cytomine-pims-0.14.0/pims/api/server.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/spectral.py` & `cytomine-pims-0.14.0/pims/api/spectral.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/thumb.py` & `cytomine-pims-0.14.0/pims/api/thumb.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/tile.py` & `cytomine-pims-0.14.0/pims/api/tile.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/__init__.py` & `cytomine-pims-0.14.0/pims/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/annotation_parameter.py` & `cytomine-pims-0.14.0/pims/api/utils/annotation_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/cytomine_auth.py` & `cytomine-pims-0.14.0/pims/api/utils/cytomine_auth.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/header.py` & `cytomine-pims-0.14.0/pims/api/utils/header.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/input_parameter.py` & `cytomine-pims-0.14.0/pims/api/utils/input_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/mimetype.py` & `cytomine-pims-0.14.0/pims/api/utils/mimetype.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/models.py` & `cytomine-pims-0.14.0/pims/api/utils/models.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/output_parameter.py` & `cytomine-pims-0.14.0/pims/api/utils/output_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/parameter.py` & `cytomine-pims-0.14.0/pims/api/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/processing_parameter.py` & `cytomine-pims-0.14.0/pims/api/utils/processing_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/range_parameter.py` & `cytomine-pims-0.14.0/pims/api/utils/range_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/utils/response.py` & `cytomine-pims-0.14.0/pims/api/utils/response.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/api/window.py` & `cytomine-pims-0.14.0/pims/api/window.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/application.py` & `cytomine-pims-0.14.0/pims/application.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/cache/__init__.py` & `cytomine-pims-0.14.0/pims/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/cache/memory.py` & `cytomine-pims-0.14.0/pims/cache/memory.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/cache/object.py` & `cytomine-pims-0.14.0/pims/cache/object.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/cache/redis.py` & `cytomine-pims-0.14.0/pims/cache/redis.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/config.py` & `cytomine-pims-0.14.0/pims/config.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/docs.py` & `cytomine-pims-0.14.0/pims/docs.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/fastapi_tweaks.py` & `cytomine-pims-0.14.0/pims/fastapi_tweaks.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/files/__init__.py` & `cytomine-pims-0.14.0/pims/files/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/files/archive.py` & `cytomine-pims-0.14.0/pims/files/archive.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/files/file.py` & `cytomine-pims-0.14.0/pims/files/file.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/files/histogram.py` & `cytomine-pims-0.14.0/pims/files/histogram.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/files/image.py` & `cytomine-pims-0.14.0/pims/files/image.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/filters/__init__.py` & `cytomine-pims-0.14.0/pims/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/filters/global_histogram.py` & `cytomine-pims-0.14.0/pims/filters/global_histogram.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/filters/pixel_color_deconvolution.py` & `cytomine-pims-0.14.0/pims/filters/pixel_color_deconvolution.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/__init__.py` & `cytomine-pims-0.14.0/pims/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/__init__.py` & `cytomine-pims-0.14.0/pims/formats/common/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/bmp.py` & `cytomine-pims-0.14.0/pims/formats/common/bmp.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/dicom.py` & `cytomine-pims-0.14.0/pims/formats/common/dicom.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/imagej.py` & `cytomine-pims-0.14.0/pims/formats/common/imagej.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/jpeg.py` & `cytomine-pims-0.14.0/pims/formats/common/jpeg.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/jpeg2000.py` & `cytomine-pims-0.14.0/pims/formats/common/jpeg2000.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/ometiff.py` & `cytomine-pims-0.14.0/pims/formats/common/ometiff.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/png.py` & `cytomine-pims-0.14.0/pims/formats/common/png.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/ppm.py` & `cytomine-pims-0.14.0/pims/formats/common/ppm.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/sis.py` & `cytomine-pims-0.14.0/pims/formats/common/sis.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/tiff.py` & `cytomine-pims-0.14.0/pims/formats/common/tiff.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/virtual.py` & `cytomine-pims-0.14.0/pims/formats/common/virtual.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/common/webp.py` & `cytomine-pims-0.14.0/pims/formats/common/webp.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/__init__.py` & `cytomine-pims-0.14.0/pims/formats/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/abstract.py` & `cytomine-pims-0.14.0/pims/formats/utils/abstract.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/checker.py` & `cytomine-pims-0.14.0/pims/formats/utils/checker.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/convertor.py` & `cytomine-pims-0.14.0/pims/formats/utils/convertor.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/engines/__init__.py` & `cytomine-pims-0.14.0/pims/formats/utils/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/engines/exiftool.py` & `cytomine-pims-0.14.0/pims/formats/utils/engines/exiftool.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/engines/omexml.py` & `cytomine-pims-0.14.0/pims/formats/utils/engines/omexml.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/engines/pil.py` & `cytomine-pims-0.14.0/pims/formats/utils/engines/pil.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/engines/tifffile.py` & `cytomine-pims-0.14.0/pims/formats/utils/engines/tifffile.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/engines/vips.py` & `cytomine-pims-0.14.0/pims/formats/utils/engines/vips.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/factories.py` & `cytomine-pims-0.14.0/pims/formats/utils/factories.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/histogram.py` & `cytomine-pims-0.14.0/pims/formats/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/parser.py` & `cytomine-pims-0.14.0/pims/formats/utils/parser.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/reader.py` & `cytomine-pims-0.14.0/pims/formats/utils/reader.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/structures/__init__.py` & `cytomine-pims-0.14.0/pims/formats/utils/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/structures/annotations.py` & `cytomine-pims-0.14.0/pims/formats/utils/structures/annotations.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/structures/metadata.py` & `cytomine-pims-0.14.0/pims/formats/utils/structures/metadata.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/structures/planes.py` & `cytomine-pims-0.14.0/pims/formats/utils/structures/planes.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/formats/utils/structures/pyramid.py` & `cytomine-pims-0.14.0/pims/formats/utils/structures/pyramid.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/importer/import_local_images.py` & `cytomine-pims-0.14.0/pims/importer/import_local_images.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/importer/importer.py` & `cytomine-pims-0.14.0/pims/importer/importer.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/importer/listeners.py` & `cytomine-pims-0.14.0/pims/importer/listeners.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/logger.py` & `cytomine-pims-0.14.0/pims/logger.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/main.py` & `cytomine-pims-0.14.0/pims/main.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/__init__.py` & `cytomine-pims-0.14.0/pims/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/adapters.py` & `cytomine-pims-0.14.0/pims/processing/adapters.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/annotations.py` & `cytomine-pims-0.14.0/pims/processing/annotations.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/colormaps.py` & `cytomine-pims-0.14.0/pims/processing/colormaps.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/histograms/__init__.py` & `cytomine-pims-0.14.0/pims/processing/histograms/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/histograms/format.py` & `cytomine-pims-0.14.0/pims/processing/histograms/format.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/histograms/utils.py` & `cytomine-pims-0.14.0/pims/processing/histograms/utils.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/image_response.py` & `cytomine-pims-0.14.0/pims/processing/image_response.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/masks.py` & `cytomine-pims-0.14.0/pims/processing/masks.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/pixels.py` & `cytomine-pims-0.14.0/pims/processing/pixels.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/processing/region.py` & `cytomine-pims-0.14.0/pims/processing/region.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/tasks/__init__.py` & `cytomine-pims-0.14.0/pims/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/tasks/queue.py` & `cytomine-pims-0.14.0/pims/tasks/queue.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/tasks/worker.py` & `cytomine-pims-0.14.0/pims/tasks/worker.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/__init__.py` & `cytomine-pims-0.14.0/pims/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/arrays.py` & `cytomine-pims-0.14.0/pims/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/background_task.py` & `cytomine-pims-0.14.0/pims/utils/background_task.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/color.py` & `cytomine-pims-0.14.0/pims/utils/color.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/concurrency.py` & `cytomine-pims-0.14.0/pims/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/copy.py` & `cytomine-pims-0.14.0/pims/utils/copy.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/dict.py` & `cytomine-pims-0.14.0/pims/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/dtypes.py` & `cytomine-pims-0.14.0/pims/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/iterables.py` & `cytomine-pims-0.14.0/pims/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/math.py` & `cytomine-pims-0.14.0/pims/utils/math.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/strings.py` & `cytomine-pims-0.14.0/pims/utils/strings.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/types.py` & `cytomine-pims-0.14.0/pims/utils/types.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/pims/utils/vips.py` & `cytomine-pims-0.14.0/pims/utils/vips.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.7/setup.py` & `cytomine-pims-0.14.0/setup.py`

 * *Files identical despite different names*

