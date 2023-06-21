# Comparing `tmp/tomoscan-1.3.0a1.tar.gz` & `tmp/tomoscan-1.3.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomoscan-1.3.0a1.tar", last modified: Wed Jun 14 12:56:44 2023, max compression
+gzip compressed data, was "tomoscan-1.3.0a2.tar", last modified: Wed Jun 21 13:51:30 2023, max compression
```

## Comparing `tomoscan-1.3.0a1.tar` & `tomoscan-1.3.0a2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.414967 tomoscan-1.3.0a1/
--rw-r--r--   0 payno    (81067) soft      (3401)     1253 2021-08-04 06:21:11.000000 tomoscan-1.3.0a1/LICENSE
--rw-r--r--   0 payno    (81067) soft      (3401)      953 2023-06-14 12:56:44.414967 tomoscan-1.3.0a1/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)      609 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/README.md
--rw-r--r--   0 payno    (81067) soft      (3401)     1213 2023-06-14 12:56:44.414967 tomoscan-1.3.0a1/setup.cfg
--rw-r--r--   0 payno    (81067) soft      (3401)     1486 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/setup.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.402967 tomoscan-1.3.0a1/tomoscan/
--rw-r--r--   0 payno    (81067) soft      (3401)       67 2022-03-24 14:18:52.000000 tomoscan-1.3.0a1/tomoscan/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/
--rw-r--r--   0 payno    (81067) soft      (3401)     1992 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)      263 2022-08-12 07:51:29.000000 tomoscan-1.3.0a1/tomoscan/esrf/edfscan.py
--rw-r--r--   0 payno    (81067) soft      (3401)      266 2022-08-12 07:51:29.000000 tomoscan-1.3.0a1/tomoscan/esrf/hdf5scan.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/identifier/
--rw-r--r--   0 payno    (81067) soft      (3401)     1765 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2926 2022-12-02 15:31:48.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/edfidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5467 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/folderidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5781 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/hdf5Identifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2302 2022-12-02 15:31:48.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/jp2kidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2732 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/rawidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3621 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/tiffidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2436 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/url_utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)      254 2023-02-20 15:01:41.000000 tomoscan-1.3.0a1/tomoscan/esrf/mock.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/scan/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2023-02-08 14:54:26.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    44250 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/edfscan.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/
--rw-r--r--   0 payno    (81067) soft      (3401)      118 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    25256 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/edfframereducer.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8542 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
--rw-r--r--   0 payno    (81067) soft      (3401)    57936 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/hdf5scan.py
--rw-r--r--   0 payno    (81067) soft      (3401)    37157 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/mock.py
--rw-r--r--   0 payno    (81067) soft      (3401)    22716 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)      257 2022-08-12 07:51:29.000000 tomoscan-1.3.0a1/tomoscan/esrf/utils.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/volume/
--rw-r--r--   0 payno    (81067) soft      (3401)     1637 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5369 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/edfvolume.py
--rw-r--r--   0 payno    (81067) soft      (3401)    19300 2023-06-02 06:46:29.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/hdf5volume.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8962 2023-05-26 12:33:10.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/jp2kvolume.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3035 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/mock.py
--rw-r--r--   0 payno    (81067) soft      (3401)    17047 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/rawvolume.py
--rw-r--r--   0 payno    (81067) soft      (3401)    15152 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/singleframebase.py
--rw-r--r--   0 payno    (81067) soft      (3401)    17517 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/tiffvolume.py
--rw-r--r--   0 payno    (81067) soft      (3401)     9222 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)    10032 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/factory.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3757 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/framereducerbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2434 2023-02-01 10:03:58.000000 tomoscan-1.3.0a1/tomoscan/identifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6006 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/io.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/nexus/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-05-03 11:55:01.000000 tomoscan-1.3.0a1/tomoscan/nexus/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.410967 tomoscan-1.3.0a1/tomoscan/nexus/paths/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-05-03 11:55:01.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)      831 2023-01-10 13:59:36.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxdetector.py
--rw-r--r--   0 payno    (81067) soft      (3401)      406 2023-01-10 13:59:36.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxinstrument.py
--rw-r--r--   0 payno    (81067) soft      (3401)      250 2023-02-01 10:03:58.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxmonitor.py
--rw-r--r--   0 payno    (81067) soft      (3401)      540 2023-01-10 13:59:36.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxsample.py
--rw-r--r--   0 payno    (81067) soft      (3401)      276 2023-01-10 13:59:36.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxsource.py
--rw-r--r--   0 payno    (81067) soft      (3401)    11151 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxtomo.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5438 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/normalization.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3214 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/progress.py
--rw-r--r--   0 payno    (81067) soft      (3401)    67019 2023-06-01 12:30:05.000000 tomoscan-1.3.0a1/tomoscan/scanbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)      303 2022-08-12 07:51:29.000000 tomoscan-1.3.0a1/tomoscan/scanfactory.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8224 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/serie.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.410967 tomoscan-1.3.0a1/tomoscan/test/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-12-06 12:48:08.000000 tomoscan-1.3.0a1/tomoscan/test/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)      266 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/conftest.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1732 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_framereducerbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)      451 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_hdf5_utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2850 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_io.py
--rw-r--r--   0 payno    (81067) soft      (3401)     7466 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_normalization.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2013 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_progress.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8996 2023-06-01 12:30:05.000000 tomoscan-1.3.0a1/tomoscan/test/test_scanbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4569 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_scanfactory.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6223 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_serie.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1611 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_tomoobject.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3704 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)    11616 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_validator.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1502 2022-12-06 12:48:08.000000 tomoscan-1.3.0a1/tomoscan/test/test_version.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2933 2023-05-26 12:33:10.000000 tomoscan-1.3.0a1/tomoscan/test/test_volume_base.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6186 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_volume_utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8574 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2341 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/tomoobject.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.410967 tomoscan-1.3.0a1/tomoscan/unitsystem/
--rw-r--r--   0 payno    (81067) soft      (3401)     1657 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2447 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/electriccurrentsystem.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3270 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/energysystem.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6542 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/metricsystem.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3165 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/timesystem.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1846 2022-12-02 15:31:48.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/unit.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1975 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/voltagesystem.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.414967 tomoscan-1.3.0a1/tomoscan/utils/
--rw-r--r--   0 payno    (81067) soft      (3401)      175 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1120 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/decorator.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2976 2023-01-05 08:34:39.000000 tomoscan-1.3.0a1/tomoscan/utils/geometry.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2666 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/hdf5.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1512 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/io.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8884 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/volume.py
--rw-r--r--   0 payno    (81067) soft      (3401)    17014 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/validator.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4346 2023-06-14 12:56:34.000000 tomoscan-1.3.0a1/tomoscan/version.py
--rw-r--r--   0 payno    (81067) soft      (3401)    21351 2023-06-14 12:55:34.000000 tomoscan-1.3.0a1/tomoscan/volumebase.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.402967 tomoscan-1.3.0a1/tomoscan.egg-info/
--rw-r--r--   0 payno    (81067) soft      (3401)      953 2023-06-14 12:56:43.000000 tomoscan-1.3.0a1/tomoscan.egg-info/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)     2741 2023-06-14 12:56:44.000000 tomoscan-1.3.0a1/tomoscan.egg-info/SOURCES.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-06-14 12:56:43.000000 tomoscan-1.3.0a1/tomoscan.egg-info/dependency_links.txt
--rw-r--r--   0 payno    (81067) soft      (3401)      300 2023-06-14 12:56:44.000000 tomoscan-1.3.0a1/tomoscan.egg-info/requires.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        9 2023-06-14 12:56:44.000000 tomoscan-1.3.0a1/tomoscan.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1253 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/LICENSE
+-rw-r--r--   0 payno     (1001) payno     (1001)      953 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)      609 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/README.md
+-rw-r--r--   0 payno     (1001) payno     (1001)     1213 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/setup.cfg
+-rw-r--r--   0 payno     (1001) payno     (1001)     1486 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/setup.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.666940 tomoscan-1.3.0a2/tomoscan/
+-rw-r--r--   0 payno     (1001) payno     (1001)       67 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.666940 tomoscan-1.3.0a2/tomoscan/esrf/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1992 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      263 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/edfscan.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      266 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/hdf5scan.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.666940 tomoscan-1.3.0a2/tomoscan/esrf/identifier/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1765 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2926 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/edfidentifier.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     5467 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/folderidentifier.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     5781 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/hdf5Identifier.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2302 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/jp2kidentifier.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2732 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/rawidentifier.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3621 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/tiffidentifier.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2431 2023-06-21 13:50:57.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/url_utils.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      254 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/mock.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/esrf/scan/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    44250 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/edfscan.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/
+-rw-r--r--   0 payno     (1001) payno     (1001)      118 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    25256 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/edfframereducer.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     8542 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    57936 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/hdf5scan.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    37157 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/mock.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    22716 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/utils.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      257 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/utils.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/esrf/volume/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1637 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     5369 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/edfvolume.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    19300 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/hdf5volume.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     8962 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/jp2kvolume.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3035 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/mock.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    17047 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/rawvolume.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    15152 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/singleframebase.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    17517 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/tiffvolume.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     9222 2023-06-21 13:43:50.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/utils.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    10032 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/factory.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3757 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/framereducerbase.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2434 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/identifier.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     6006 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/io.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/nexus/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/nexus/paths/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      831 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxdetector.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      406 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxinstrument.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      250 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxmonitor.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      540 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxsample.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      276 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxsource.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    11151 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxtomo.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     5438 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/normalization.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3214 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/progress.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    67019 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/scanbase.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      303 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/scanfactory.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     8224 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/serie.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.674940 tomoscan-1.3.0a2/tomoscan/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      266 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/conftest.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1732 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_framereducerbase.py
+-rw-r--r--   0 payno     (1001) payno     (1001)      451 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_hdf5_utils.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2850 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_io.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     7466 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_normalization.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2013 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_progress.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     8996 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_scanbase.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4569 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_scanfactory.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     6223 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_serie.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1611 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_tomoobject.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3704 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_utils.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    11616 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_validator.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1502 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_version.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2933 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_volume_base.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     6186 2023-06-21 13:43:50.000000 tomoscan-1.3.0a2/tomoscan/test/test_volume_utils.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     8574 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/utils.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2341 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/tomoobject.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/tomoscan/unitsystem/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1657 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2447 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/electriccurrentsystem.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3270 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/energysystem.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     6542 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/metricsystem.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3165 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/timesystem.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1846 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/unit.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1975 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/voltagesystem.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/tomoscan/utils/
+-rw-r--r--   0 payno     (1001) payno     (1001)      175 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1120 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/decorator.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2976 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/geometry.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2666 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/hdf5.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1512 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/io.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     8884 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/volume.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    17014 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/validator.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4346 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/version.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    21351 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/volumebase.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.666940 tomoscan-1.3.0a2/tomoscan.egg-info/
+-rw-r--r--   0 payno     (1001) payno     (1001)      953 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)     2741 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)      300 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/requires.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        9 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/top_level.txt
```

### Comparing `tomoscan-1.3.0a1/LICENSE` & `tomoscan-1.3.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/PKG-INFO` & `tomoscan-1.3.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.3.0a1
+Version: 1.3.0a2
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.3.0a1/README.md` & `tomoscan-1.3.0a2/README.md`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/setup.cfg` & `tomoscan-1.3.0a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/setup.py` & `tomoscan-1.3.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/__init__.py` & `tomoscan-1.3.0a2/tomoscan/esrf/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/identifier/__init__.py` & `tomoscan-1.3.0a2/tomoscan/esrf/identifier/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/identifier/edfidentifier.py` & `tomoscan-1.3.0a2/tomoscan/esrf/identifier/edfidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/identifier/folderidentifier.py` & `tomoscan-1.3.0a2/tomoscan/esrf/identifier/folderidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/identifier/hdf5Identifier.py` & `tomoscan-1.3.0a2/tomoscan/esrf/identifier/hdf5Identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/identifier/jp2kidentifier.py` & `tomoscan-1.3.0a2/tomoscan/esrf/identifier/jp2kidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/identifier/rawidentifier.py` & `tomoscan-1.3.0a2/tomoscan/esrf/identifier/rawidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/identifier/tiffidentifier.py` & `tomoscan-1.3.0a2/tomoscan/esrf/identifier/tiffidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/identifier/url_utils.py` & `tomoscan-1.3.0a2/tomoscan/esrf/identifier/url_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 from typing import Iterable, Tuple
 
 
 class UrlSettings:
     FILE_PATH_KEY = "file_path"
-    DATA_PATH_KEY = "data_path"
+    DATA_PATH_KEY = "path"
     FILE_PREFIX = "file_prefix"
 
 
 def split_query(query: str) -> dict:
     result = dict()
     for s in query.split("&"):
         if not s:
```

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/scan/edfscan.py` & `tomoscan-1.3.0a2/tomoscan/esrf/scan/edfscan.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/edfframereducer.py` & `tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/edfframereducer.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/hdf5framereducer.py` & `tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/hdf5framereducer.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/scan/hdf5scan.py` & `tomoscan-1.3.0a2/tomoscan/esrf/scan/hdf5scan.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/scan/mock.py` & `tomoscan-1.3.0a2/tomoscan/esrf/scan/mock.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/scan/utils.py` & `tomoscan-1.3.0a2/tomoscan/esrf/scan/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/__init__.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/edfvolume.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/edfvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/hdf5volume.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/hdf5volume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/jp2kvolume.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/jp2kvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/mock.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/mock.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/rawvolume.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/rawvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/singleframebase.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/singleframebase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/tiffvolume.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/tiffvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/esrf/volume/utils.py` & `tomoscan-1.3.0a2/tomoscan/esrf/volume/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/factory.py` & `tomoscan-1.3.0a2/tomoscan/factory.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/framereducerbase.py` & `tomoscan-1.3.0a2/tomoscan/framereducerbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/identifier.py` & `tomoscan-1.3.0a2/tomoscan/identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/io.py` & `tomoscan-1.3.0a2/tomoscan/io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/nexus/paths/nxdetector.py` & `tomoscan-1.3.0a2/tomoscan/nexus/paths/nxdetector.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/nexus/paths/nxsample.py` & `tomoscan-1.3.0a2/tomoscan/nexus/paths/nxsample.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/nexus/paths/nxtomo.py` & `tomoscan-1.3.0a2/tomoscan/nexus/paths/nxtomo.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/normalization.py` & `tomoscan-1.3.0a2/tomoscan/normalization.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/progress.py` & `tomoscan-1.3.0a2/tomoscan/progress.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/scanbase.py` & `tomoscan-1.3.0a2/tomoscan/scanbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/serie.py` & `tomoscan-1.3.0a2/tomoscan/serie.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_framereducerbase.py` & `tomoscan-1.3.0a2/tomoscan/test/test_framereducerbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_io.py` & `tomoscan-1.3.0a2/tomoscan/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_normalization.py` & `tomoscan-1.3.0a2/tomoscan/test/test_normalization.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_progress.py` & `tomoscan-1.3.0a2/tomoscan/test/test_progress.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_scanbase.py` & `tomoscan-1.3.0a2/tomoscan/test/test_scanbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_scanfactory.py` & `tomoscan-1.3.0a2/tomoscan/test/test_scanfactory.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_serie.py` & `tomoscan-1.3.0a2/tomoscan/test/test_serie.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_tomoobject.py` & `tomoscan-1.3.0a2/tomoscan/test/test_tomoobject.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_utils.py` & `tomoscan-1.3.0a2/tomoscan/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_validator.py` & `tomoscan-1.3.0a2/tomoscan/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_version.py` & `tomoscan-1.3.0a2/tomoscan/test/test_version.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_volume_base.py` & `tomoscan-1.3.0a2/tomoscan/test/test_volume_base.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/test_volume_utils.py` & `tomoscan-1.3.0a2/tomoscan/test/test_volume_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/test/utils.py` & `tomoscan-1.3.0a2/tomoscan/test/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/tomoobject.py` & `tomoscan-1.3.0a2/tomoscan/tomoobject.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/unitsystem/__init__.py` & `tomoscan-1.3.0a2/tomoscan/unitsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/unitsystem/electriccurrentsystem.py` & `tomoscan-1.3.0a2/tomoscan/unitsystem/electriccurrentsystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/unitsystem/energysystem.py` & `tomoscan-1.3.0a2/tomoscan/unitsystem/energysystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/unitsystem/metricsystem.py` & `tomoscan-1.3.0a2/tomoscan/unitsystem/metricsystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/unitsystem/timesystem.py` & `tomoscan-1.3.0a2/tomoscan/unitsystem/timesystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/unitsystem/unit.py` & `tomoscan-1.3.0a2/tomoscan/unitsystem/unit.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/unitsystem/voltagesystem.py` & `tomoscan-1.3.0a2/tomoscan/unitsystem/voltagesystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/utils/decorator.py` & `tomoscan-1.3.0a2/tomoscan/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/utils/geometry.py` & `tomoscan-1.3.0a2/tomoscan/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/utils/hdf5.py` & `tomoscan-1.3.0a2/tomoscan/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/utils/io.py` & `tomoscan-1.3.0a2/tomoscan/utils/io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/utils/volume.py` & `tomoscan-1.3.0a2/tomoscan/utils/volume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/validator.py` & `tomoscan-1.3.0a2/tomoscan/validator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan/version.py` & `tomoscan-1.3.0a2/tomoscan/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 3
 MICRO = 0
 RELEV = "alpha"  # <16
-SERIAL = 1  # <16
+SERIAL = 2  # <16
 
 date = __date__
 
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
 )
```

### Comparing `tomoscan-1.3.0a1/tomoscan/volumebase.py` & `tomoscan-1.3.0a2/tomoscan/volumebase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a1/tomoscan.egg-info/PKG-INFO` & `tomoscan-1.3.0a2/tomoscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.3.0a1
+Version: 1.3.0a2
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.3.0a1/tomoscan.egg-info/SOURCES.txt` & `tomoscan-1.3.0a2/tomoscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

