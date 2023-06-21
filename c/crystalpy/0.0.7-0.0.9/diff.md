# Comparing `tmp/crystalpy-0.0.7.tar.gz` & `tmp/crystalpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crystalpy-0.0.7.tar", last modified: Tue Jun 14 13:29:52 2022, max compression
+gzip compressed data, was "dist/crystalpy-0.0.9.tar", last modified: Mon Nov 14 13:32:08 2022, max compression
```

## Comparing `crystalpy-0.0.7.tar` & `crystalpy-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-06-14 13:29:52.000000 crystalpy-0.0.7/
--rw-r--r--   0 srio      (4230) soft      (3401)     1068 2021-11-08 15:03:38.000000 crystalpy-0.0.7/LICENSE
--rw-r--r--   0 srio      (4230) soft      (3401)      308 2022-06-14 13:29:52.000000 crystalpy-0.0.7/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)      509 2021-11-08 15:03:38.000000 crystalpy-0.0.7/README.md
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy/diffraction/
--rw-r--r--   0 srio      (4230) soft      (3401)     2291 2021-11-08 15:38:40.000000 crystalpy-0.0.7/crystalpy/diffraction/ComplexAmplitude.py
--rw-r--r--   0 srio      (4230) soft      (3401)    23823 2022-06-14 13:28:59.000000 crystalpy-0.0.7/crystalpy/diffraction/Diffraction.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1757 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/diffraction/DiffractionExceptions.py
--rw-r--r--   0 srio      (4230) soft      (3401)    10211 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/diffraction/DiffractionResult.py
--rw-r--r--   0 srio      (4230) soft      (3401)     7028 2022-01-18 11:57:44.000000 crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetup.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21316 2022-01-28 08:37:56.000000 crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupAbstract.py
--rw-r--r--   0 srio      (4230) soft      (3401)     6426 2022-04-26 09:25:46.000000 crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupDabax.py
--rw-r--r--   0 srio      (4230) soft      (3401)    12013 2022-01-28 08:37:56.000000 crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupShadowPreprocessorV1.py
--rw-r--r--   0 srio      (4230) soft      (3401)     8716 2022-01-28 08:37:56.000000 crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupShadowPreprocessorV2.py
--rw-r--r--   0 srio      (4230) soft      (3401)     8376 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupSweeps.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2379 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/diffraction/GeometryType.py
--rw-r--r--   0 srio      (4230) soft      (3401)    22798 2022-06-14 13:28:59.000000 crystalpy-0.0.7/crystalpy/diffraction/PerfectCrystalDiffraction.py
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/diffraction/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy/examples/
--rw-r--r--   0 srio      (4230) soft      (3401)     8486 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/examples/PlotData1D.py
--rw-r--r--   0 srio      (4230) soft      (3401)    15040 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/examples/Si111.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4246 2021-11-22 13:05:42.000000 crystalpy-0.0.7/crystalpy/examples/Si111_energy_scan.py
--rw-r--r--   0 srio      (4230) soft      (3401)    10354 2021-11-18 14:07:13.000000 crystalpy-0.0.7/crystalpy/examples/Si111_layered.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3510 2022-01-17 11:33:34.000000 crystalpy-0.0.7/crystalpy/examples/Si111_simple.py
--rw-r--r--   0 srio      (4230) soft      (3401)    23511 2022-04-26 09:25:46.000000 crystalpy-0.0.7/crystalpy/examples/Si111_simple_xraylib_dabax_comparison.py
--rw-r--r--   0 srio      (4230) soft      (3401)    12102 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/examples/Values.py
--rw-r--r--   0 srio      (4230) soft      (3401)     6029 2022-04-26 09:25:46.000000 crystalpy-0.0.7/crystalpy/examples/YB66.py
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/examples/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21077 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/examples/check_against_xoppy_crystal.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21676 2022-01-18 14:46:46.000000 crystalpy-0.0.7/crystalpy/examples/check_against_xoppy_crystal_including_shadow_proprocessor.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2664 2022-01-18 11:40:01.000000 crystalpy-0.0.7/crystalpy/examples/check_structure_factor.py
--rw-r--r--   0 srio      (4230) soft      (3401)    14570 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/examples/main.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy/polarization/
--rw-r--r--   0 srio      (4230) soft      (3401)     2615 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/polarization/CrystalPhasePlate.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3408 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/polarization/MuellerDiffraction.py
--rw-r--r--   0 srio      (4230) soft      (3401)     8236 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/polarization/MuellerMatrix.py
--rw-r--r--   0 srio      (4230) soft      (3401)     6022 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/polarization/MuellerResult.py
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/polarization/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy/tests/
--rw-r--r--   0 srio      (4230) soft      (3401)     2600 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/tests/PyCrystalTests.py
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/tests/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy/util/
--rw-r--r--   0 srio      (4230) soft      (3401)     3555 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/util/ComplexAmplitudePhoton.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2207 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/util/ComplexAmplitudePhotonBunch.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2756 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/util/Photon.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4285 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/util/PhotonBunch.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2940 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/util/PolarizedPhoton.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2164 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/util/PolarizedPhotonBunch.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2790 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/util/StokesVector.py
--rw-r--r--   0 srio      (4230) soft      (3401)     8108 2022-01-17 08:33:28.000000 crystalpy-0.0.7/crystalpy/util/Vector.py
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.7/crystalpy/util/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy.egg-info/
--rw-r--r--   0 srio      (4230) soft      (3401)      308 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy.egg-info/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)     1900 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy.egg-info/SOURCES.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy.egg-info/dependency_links.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       25 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy.egg-info/requires.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       10 2022-06-14 13:29:52.000000 crystalpy-0.0.7/crystalpy.egg-info/top_level.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       38 2022-06-14 13:29:52.000000 crystalpy-0.0.7/setup.cfg
--rw-r--r--   0 srio      (4230) soft      (3401)      939 2022-06-14 13:27:10.000000 crystalpy-0.0.7/setup.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-11-14 13:32:08.000000 crystalpy-0.0.9/
+-rw-r--r--   0 srio      (4230) soft      (3401)     1068 2021-11-08 15:03:38.000000 crystalpy-0.0.9/LICENSE
+-rw-r--r--   0 srio      (4230) soft      (3401)      308 2022-11-14 13:32:08.000000 crystalpy-0.0.9/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)      509 2021-11-08 15:03:38.000000 crystalpy-0.0.9/README.md
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy/diffraction/
+-rw-r--r--   0 srio      (4230) soft      (3401)     2291 2021-11-08 15:38:40.000000 crystalpy-0.0.9/crystalpy/diffraction/ComplexAmplitude.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    24092 2022-11-14 13:17:55.000000 crystalpy-0.0.9/crystalpy/diffraction/Diffraction.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1757 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/diffraction/DiffractionExceptions.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    10211 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/diffraction/DiffractionResult.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     7028 2022-01-18 11:57:44.000000 crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetup.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21316 2022-01-28 08:37:56.000000 crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupAbstract.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     6426 2022-04-26 09:25:46.000000 crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupDabax.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    12013 2022-01-28 08:37:56.000000 crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupShadowPreprocessorV1.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     8716 2022-01-28 08:37:56.000000 crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupShadowPreprocessorV2.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     8376 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupSweeps.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2379 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/diffraction/GeometryType.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    32749 2022-11-14 10:44:42.000000 crystalpy-0.0.9/crystalpy/diffraction/PerfectCrystalDiffraction.py
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/diffraction/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy/examples/
+-rw-r--r--   0 srio      (4230) soft      (3401)     8486 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/examples/PlotData1D.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    15040 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/examples/Si111.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4246 2021-11-22 13:05:42.000000 crystalpy-0.0.9/crystalpy/examples/Si111_energy_scan.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5139 2022-11-14 11:12:49.000000 crystalpy-0.0.9/crystalpy/examples/Si111_guigay.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4381 2022-10-06 13:50:10.000000 crystalpy-0.0.9/crystalpy/examples/Si111_guigay_map_inside_crystal.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    10354 2021-11-18 14:07:13.000000 crystalpy-0.0.9/crystalpy/examples/Si111_layered.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3510 2022-01-17 11:33:34.000000 crystalpy-0.0.9/crystalpy/examples/Si111_simple.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    23511 2022-04-26 09:25:46.000000 crystalpy-0.0.9/crystalpy/examples/Si111_simple_xraylib_dabax_comparison.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    12102 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/examples/Values.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     6029 2022-04-26 09:25:46.000000 crystalpy-0.0.9/crystalpy/examples/YB66.py
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/examples/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21077 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/examples/check_against_xoppy_crystal.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21676 2022-01-18 14:46:46.000000 crystalpy-0.0.9/crystalpy/examples/check_against_xoppy_crystal_including_shadow_proprocessor.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2664 2022-01-18 11:40:01.000000 crystalpy-0.0.9/crystalpy/examples/check_structure_factor.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    14570 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/examples/main.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy/polarization/
+-rw-r--r--   0 srio      (4230) soft      (3401)     2615 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/polarization/CrystalPhasePlate.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3408 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/polarization/MuellerDiffraction.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     8236 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/polarization/MuellerMatrix.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     6022 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/polarization/MuellerResult.py
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/polarization/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy/tests/
+-rw-r--r--   0 srio      (4230) soft      (3401)     2600 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/tests/PyCrystalTests.py
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/tests/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)     3555 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/util/ComplexAmplitudePhoton.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2207 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/util/ComplexAmplitudePhotonBunch.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2756 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/util/Photon.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4285 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/util/PhotonBunch.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2940 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/util/PolarizedPhoton.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2164 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/util/PolarizedPhotonBunch.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2790 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/util/StokesVector.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     8108 2022-01-17 08:33:28.000000 crystalpy-0.0.9/crystalpy/util/Vector.py
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2021-11-08 15:03:38.000000 crystalpy-0.0.9/crystalpy/util/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy.egg-info/
+-rw-r--r--   0 srio      (4230) soft      (3401)      308 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy.egg-info/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)     1989 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       25 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy.egg-info/requires.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       10 2022-11-14 13:32:08.000000 crystalpy-0.0.9/crystalpy.egg-info/top_level.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       38 2022-11-14 13:32:08.000000 crystalpy-0.0.9/setup.cfg
+-rw-r--r--   0 srio      (4230) soft      (3401)      939 2022-11-14 13:31:39.000000 crystalpy-0.0.9/setup.py
```

### Comparing `crystalpy-0.0.7/LICENSE` & `crystalpy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/ComplexAmplitude.py` & `crystalpy-0.0.9/crystalpy/diffraction/ComplexAmplitude.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/Diffraction.py` & `crystalpy-0.0.9/crystalpy/diffraction/Diffraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             if diffraction_setup.asymmetryAngle() <= bragg_angle:
                 raise TransmissionImpossibleException()
 
 
     def _perfectCrystalForEnergy(self, diffraction_setup, energy):
 
         # Retrieve bragg angle.
-        angle_bragg = diffraction_setup.bragg_angle(energy)
+        angle_bragg = diffraction_setup.angleBragg(energy)
 
         # Get structure factors for all relevant lattice vectors 0,H,H_bar.
         if False: # this is "commented" by srio to speed it up!
             F_0 = diffraction_setup.F0(energy)
             F_H = diffraction_setup.FH(energy)
             F_H_bar = diffraction_setup.FH_bar(energy)
 
@@ -211,15 +211,15 @@
 
             # Log the structure factors.
             if self.isDebug:
                 self.logStructureFactorsPsi(F_0, F_H, F_H_bar)
 
 
         # Retrieve lattice spacing d.
-        d_spacing = diffraction_setup.d_spacing() * 1e-10
+        d_spacing = diffraction_setup.dSpacing() * 1e-10
 
         # Calculate the Bragg normal B_H.
         normal_bragg = diffraction_setup.normalBragg()
 
         # Calculate the surface normal n.
         normal_surface = diffraction_setup.normalSurface()
 
@@ -247,15 +247,15 @@
                                                     psi_H=psi_H,
                                                     psi_H_bar=psi_H_bar,
                                                     thickness=diffraction_setup.thickness(),
                                                     d_spacing=d_spacing)
 
         return perfect_crystal
 
-    def _calculateDiffractionForEnergy(self, diffraction_setup, energy, result):
+    def _calculateDiffractionForEnergy(self, diffraction_setup, energy, result, method=0):
         """
         Calculates the diffraction/transmission given by the setup.
         :param diffraction_setup: The diffraction setup.
         :return: DiffractionResult representing this setup.
         """
         # Get PerfectCrystal instance for the current energy.
         if not isinstance(diffraction_setup,DiffractionSetupSweeps):
@@ -272,15 +272,15 @@
             self._onProgressEveryTenPercent(index, diffraction_setup.angleDeviationPoints())
 
             # Calculate deviated incoming photon.
             photon_direction = diffraction_setup.incomingPhotonDirection(energy, deviation)
             photon_in = Photon(energy, photon_direction)
 
             # Calculate diffraction for current incoming photon.
-            result_deviation = perfect_crystal.calculateDiffraction(photon_in)
+            result_deviation = perfect_crystal.calculateDiffraction(photon_in, method=method)
 
             # Calculate polarization difference between pi and sigma polarization.
             polarization_difference = result_deviation["P"] / result_deviation["S"]
 
             # Add result of current deviation.
             result.add(energy,
                        deviation,
@@ -290,29 +290,30 @@
 
         # Raise calculation end.
         self._onCalculationEnd()
 
         # Return diffraction results.
         return result
 
-    def calculateDiffraction(self, diffraction_setup):
+    def calculateDiffraction(self, diffraction_setup, method=0):
         """
         Calculates the diffraction/transmission given by the setup.
         :param diffraction_setup: The diffraction setup.
+        :method: 0=Zachariasen, 1=Guigay
         :return: DiffractionResult representing this setup.
         """
 
         if not isinstance(diffraction_setup,DiffractionSetupSweeps):
             raise Exception("Input object must be of type DiffractionSetupSweeps")
 
         # Create DiffractionResult instance.
         result = DiffractionResult(diffraction_setup, 0.0)
 
         for energy in diffraction_setup.energies():
-            self._calculateDiffractionForEnergy(diffraction_setup, energy, result)
+            self._calculateDiffractionForEnergy(diffraction_setup, energy, result, method=method)
 
         # Return diffraction results.
         return result
 
     #TODO remove? where is used??
 
     # def calculateDiffractionForPhotonBunch(self, diffraction_setup, photon_bunch):
@@ -392,28 +393,28 @@
                                                     psi_H=psi_H,
                                                     psi_H_bar=psi_H_bar,
                                                     thickness=diffraction_setup.thickness(),
                                                     d_spacing=d_spacing)
 
         return perfect_crystal
 
-    def calculateDiffractedPolarizedPhoton(self, diffraction_setup, incoming_polarized_photon, inclination_angle):
+    def calculateDiffractedPolarizedPhoton(self, diffraction_setup, incoming_polarized_photon, inclination_angle, method=0):
         """
         Calculates the diffraction/transmission given by the setup.
         :param diffraction_setup: The diffraction setup.
         :return: PhotonBunch object made up of diffracted/transmitted photons.
         """
         # Retrieve the incoming Stokes vector.
         incoming_stokes_vector = incoming_polarized_photon.stokesVector()
 
         # Get PerfectCrystal instance for the current photon.
         perfect_crystal = self._perfectCrystalForPhoton(diffraction_setup, incoming_polarized_photon)
 
         # Calculate diffraction for current incoming photon.
-        complex_amplitudes = perfect_crystal.calculateDiffraction(incoming_polarized_photon)
+        complex_amplitudes = perfect_crystal.calculateDiffraction(incoming_polarized_photon, method=method)
 
         # Calculate outgoing Photon.
         outgoing_photon = perfect_crystal._calculatePhotonOut(incoming_polarized_photon)
 
         # Calculate intensities and phases of the crystal  reflectivities or transmitivities
         intensity_pi = complex_amplitudes["P"].intensity()
         intensity_sigma = complex_amplitudes["S"].intensity()
@@ -435,15 +436,15 @@
         outgoing_polarized_photon = PolarizedPhoton(energy_in_ev=outgoing_photon.energy(),
                                                     direction_vector=outgoing_photon.unitDirectionVector(),
                                                     stokes_vector=outgoing_stokes_vector)
 
         return outgoing_polarized_photon
 
 
-    def calculateDiffractedPolarizedPhotonBunch(self, diffraction_setup, incoming_bunch, inclination_angle):
+    def calculateDiffractedPolarizedPhotonBunch(self, diffraction_setup, incoming_bunch, inclination_angle, method=0):
         """
         Calculates the diffraction/transmission given by the setup.
         :param diffraction_setup: The diffraction setup.
         :return: PhotonBunch object made up of diffracted/transmitted photons.
         """
         # Create PhotonBunch instance.
         outgoing_bunch = PolarizedPhotonBunch([])
@@ -459,42 +460,43 @@
         self._onCalculationStart()
 
         for index, polarized_photon in enumerate(incoming_bunch):
 
             # Raise OnProgress event if progressed by 10 percent.
             self._onProgressEveryTenPercent(index, len(incoming_bunch))
 
-            outgoing_polarized_photon = self.calculateDiffractedPolarizedPhoton(diffraction_setup, polarized_photon, inclination_angle)
+            outgoing_polarized_photon = self.calculateDiffractedPolarizedPhoton(diffraction_setup, polarized_photon,
+                                                                                inclination_angle, method=method)
             # Add result of current deviation.
             outgoing_bunch.addPhoton(outgoing_polarized_photon)
 
         # Raise calculation end.
         self._onCalculationEnd()
 
         # Return diffraction results.
         return outgoing_bunch
 
     # calculate complex reflectivity and transmitivity
-    def calculateDiffractedComplexAmplitudes(self, diffraction_setup, incoming_photon):
+    def calculateDiffractedComplexAmplitudes(self, diffraction_setup, incoming_photon, method=0):
 
         # Get PerfectCrystal instance for the current photon.
         perfect_crystal = self._perfectCrystalForPhoton(diffraction_setup, incoming_photon)
 
         # Calculate diffraction for current incoming photon.
-        complex_amplitudes = perfect_crystal.calculateDiffraction(incoming_photon)
+        complex_amplitudes = perfect_crystal.calculateDiffraction(incoming_photon, method=method)
 
         return complex_amplitudes
 
     # using ComplexAmplitudePhoton
-    def calculateDiffractedComplexAmplitudePhoton(self, diffraction_setup,photon):
+    def calculateDiffractedComplexAmplitudePhoton(self, diffraction_setup,photon, method=0):
 
         # Get PerfectCrystal instance for the current photon.
         perfect_crystal = self._perfectCrystalForPhoton(diffraction_setup, photon)
 
-        coeffs = self.calculateDiffractedComplexAmplitudes(diffraction_setup,photon)
+        coeffs = self.calculateDiffractedComplexAmplitudes(diffraction_setup,photon, method=method)
 
         # Calculate outgoing Photon.
         outgoing_photon = perfect_crystal._calculatePhotonOut(photon)
         # apply reflectivities
         outgoing_photon.rescaleEsigma(coeffs["S"])
         outgoing_photon.rescaleEpi(coeffs["P"])
```

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/DiffractionExceptions.py` & `crystalpy-0.0.9/crystalpy/diffraction/DiffractionExceptions.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/DiffractionResult.py` & `crystalpy-0.0.9/crystalpy/diffraction/DiffractionResult.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetup.py` & `crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetup.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupAbstract.py` & `crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupAbstract.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupDabax.py` & `crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupDabax.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupShadowPreprocessorV1.py` & `crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupShadowPreprocessorV1.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupShadowPreprocessorV2.py` & `crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupShadowPreprocessorV2.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/DiffractionSetupSweeps.py` & `crystalpy-0.0.9/crystalpy/diffraction/DiffractionSetupSweeps.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/GeometryType.py` & `crystalpy-0.0.9/crystalpy/diffraction/GeometryType.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/diffraction/PerfectCrystalDiffraction.py` & `crystalpy-0.0.9/crystalpy/diffraction/PerfectCrystalDiffraction.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Calculates crystal diffraction according to Zachariasen's representation of the dynamic theory of crystal diffraction
 for perfect crystals.
 Except for energy all units are in SI. Energy is in eV.
 """
 
-from numpy import pi, cos, sqrt
+import numpy
+from numpy import pi, cos, sin, sqrt, abs, exp, tanh, sinh, cosh, imag, real
 
 from crystalpy.diffraction.ComplexAmplitude import ComplexAmplitude
 from crystalpy.util.Photon import Photon
 from crystalpy.diffraction.GeometryType import BraggDiffraction, LaueDiffraction, BraggTransmission, LaueTransmission
 
 # Use mpmath if possible. Otherwise use native cmath.
 try:
@@ -328,45 +329,62 @@
                                 pi * 0.5 - photon_out.unitDirectionVector().angle(self.braggNormal()))))
             self.logDebug("photon_in direction" + str(photon_in.unitDirectionVector().components()))
             self.logDebug("photon_out direction" + str(photon_out.unitDirectionVector().components()))
 
         # Return outgoing photon.
         return photon_out
 
+
     def _calculateZacAlpha(self, photon_in):
         """
         Calculates alpha ("refraction index difference between waves in the crystal") as defined in Zachariasen [3-114b].
         :param photon_in: Incoming photon.
         :return: alpha.
         """
         # Calculate scalar product k_0 and B_H.
         k_0_times_B_h = photon_in.wavevector().scalarProduct(self.braggNormal())
 
         # Get norm k_0.
         wavenumber = photon_in.wavenumber()
 
         # Calculate alpha.
         zac_alpha = (wavenumber ** -2) * (self.braggNormal().norm() ** 2 + 2 * k_0_times_B_h)
+        # we defined theta = theta_b + deviation (for symmetric Bragg), therefore the
+        # approximated value of zac_alpha (compare eqs 3.116)  = 2 (theta_b-theta) sin(2 theta_b) =
+        # = 2 (-deviation) * sin(2 theta_b)
 
         # Return alpha.
         return zac_alpha
 
     def _calculateZacB(self, photon_in, photon_out):
         """
         Calculates asymmetry ratio b as defined in Zachariasen [3-115].
         :param photon_in: Incoming photon.
         :param photon_out: Outgoing photon.
         :return: Asymmetry ratio b.
         """
+        # TODO: revise this algorithm, it is not exactly as in Zachariasen [3-115]
         numerator   = self.surface_normal().scalarProduct(photon_in.wavevector())
         denominator = self.surface_normal().scalarProduct(photon_out.wavevector())
         zac_b = numerator / denominator
 
         return zac_b
 
+    def _calculateGuigayB(self, photon_in, photon_out):
+        """
+        Calculates asymmetry ratio b as defined in Guigay.
+        :param photon_in: Incoming photon.
+        :param photon_out: Outgoing photon.
+        :return: Asymmetry ratio b.
+        Note that this b value is not standard, as it changes when b changes
+        """
+        numerator   = self.surface_normal().scalarProduct(photon_in.wavevector())
+        denominator = self.surface_normal().scalarProduct(photon_out.wavevector())
+        return numerator / denominator
+
     def _calculateZacQ(self, zac_b, effective_psi_h, effective_psi_h_bar):
         """
         Calculates q as defined in Zachariasen [3-123].
         :param zac_b: Asymmetry ratio b as defined in Zachariasen [3-115].
         :param effective_psi_h: Effective PsiH (depending of polarisation. See text following [3.-139]).
         :param effective_psi_h_bar: Effective PsiHBar (depending of polarisation. See text following [3.-139]).
         :return: q.
@@ -498,15 +516,33 @@
         effective_psi_h_bar = self.PsiHBar() * cos(2 * self.braggAngle())
 
         zac_q = self._calculateZacQ(zac_b, effective_psi_h, effective_psi_h_bar)
 
         return self._calculateComplexAmplitude(photon_in, zac_q, zac_z, gamma_0,
                                                effective_psi_h_bar)
 
-    def calculateDiffraction(self, photon_in):
+    def calculateDiffraction(self,
+                             photon_in,
+                             method=0, # 0=Zachariasen, 1=Guigay
+                             ):
+        """
+        Calculate diffraction for incoming photon.
+        :param photon_in: Incoming photon.
+        :return: Complex amplitude of the diffraction.
+        """
+
+        if method == 0:
+            # print(">>>> Using Zachariasen equations...")
+            return self.calculateDiffractionZachariasen(photon_in)
+        else:
+            # print(">>>> Using Guigay equations...")
+            return self.calculateDiffractionGuigay(photon_in)
+
+
+    def calculateDiffractionZachariasen(self, photon_in):
         """
         Calculate diffraction for incoming photon.
         :param photon_in: Incoming photon.
         :return: Complex amplitude of the diffraction.
         """
         # Initialize return variable.
         result = {"S": None,
@@ -544,18 +580,201 @@
         # If debugging output is turned on.
         if self.isDebug:
             self._logMembers(zac_b, zac_alpha, photon_in, photon_out, result)
 
         # Returns the complex amplitudes.
         return result
 
+    def calculateDiffractionGuigay(self, photon_in, debug=0, s_ratio=None):
+        """
+        Calculate diffraction for incoming photon.
+        :param photon_in: Incoming photon.
+        :return: Complex amplitude of the diffraction.
+        """
+        # Initialize return variable.
+        result = {"S": None,
+                  "P": None}
+
+        # Calculate photon out.
+        photon_out = self._calculatePhotonOut(photon_in)
+
+        # Calculate crystal field refraction index difference.
+        # Note that Guigay's definition of alpha has the opposite sign as in Zachariasen!
+        zac_guigay = - self._calculateZacAlpha(photon_in)
+        if debug: print("zac_guigay: ", zac_guigay)
+
+        # Calculate asymmetry ratio. Note that this is not a constant!
+        if debug:
+            zac_b = self._calculateZacB(photon_in, photon_out)
+            print("zac_b: ", zac_b)
+
+        h = 2 * photon_in.wavevector().norm() * numpy.sin(self._bragg_angle)
+        H = (self.braggNormal().getNormalizedVector()).scalarMultiplication(h)
+        if debug: print("H: ",H.components())
+
+        KH = photon_in.wavevector().addVector(H)
+        photon_outG = Photon(energy_in_ev=photon_in.energy(), direction_vector=KH)
+        if debug:
+            guigay_b = self._calculateGuigayB(photon_in, photon_outG)
+            print("guigay_b: ", guigay_b)
+
+        gamma_0 = self._calculateGamma(photon_in)
+        gamma_H = self._calculateGamma(photon_outG)
+        guigay_b = gamma_0 / gamma_H
+        if debug: print("guigay_b: ", guigay_b)
+
+
+        T = self.thickness() / gamma_0
+
+        effective_psi_0 = numpy.conjugate(self.Psi0())  # I(Psi0) > 0 (for absorption!!)
+        w = guigay_b * (zac_guigay / 2) + effective_psi_0 * (guigay_b - 1) / 2
+        omega = numpy.pi / photon_in.wavelength() * w
+
+        if self.geometryType() == BraggDiffraction():
+            if s_ratio is None:
+                s = 0.0
+            else:
+                s = T * s_ratio
+            # sigma polarization
+            effective_psi_h = numpy.conjugate(self.PsiH())
+            effective_psi_h_bar = numpy.conjugate(self.PsiHBar())
+            SQ = sqrt(guigay_b * effective_psi_h * effective_psi_h_bar + w ** 2)
+            uh = effective_psi_h * pi / photon_in.wavelength()
+            u0 = effective_psi_0 * pi / photon_in.wavelength()
+            a = pi / photon_in.wavelength() * SQ
+
+            complex_amplitude_s = 1j * guigay_b * uh * numpy.sin(a * s - a * T) / \
+                                (a * numpy.cos(a * T) + 1j * omega * numpy.sin(a * T)) * \
+                                numpy.exp(1j * s * (omega + u0))
+
+            # pi polarization
+            effective_psi_h = numpy.conjugate(self.PsiH()) * cos(2 * self.braggAngle())
+            effective_psi_h_bar = numpy.conjugate(self.PsiHBar()) * cos(2 * self.braggAngle())
+            SQ = sqrt(guigay_b * effective_psi_h * effective_psi_h_bar + w ** 2)
+            uh = effective_psi_h * pi / photon_in.wavelength()
+            u0 = effective_psi_0 * pi / photon_in.wavelength()
+            a = pi / photon_in.wavelength() * SQ
+
+            complex_amplitude_p = 1j * guigay_b * uh * numpy.sin( a * s - a * T) / \
+                                (a * numpy.cos(a * T) + 1j * omega * numpy.sin(a * T)) * \
+                                numpy.exp(1j * s * (omega + u0))
+
+        elif self.geometryType() == BraggTransmission():
+            if s_ratio is None:
+                s = T
+            else:
+                s = T * s_ratio
+            # sigma polarization
+            effective_psi_h = numpy.conjugate(self.PsiH())
+            effective_psi_h_bar = numpy.conjugate(self.PsiHBar())
+            SQ = sqrt(guigay_b * effective_psi_h * effective_psi_h_bar + w ** 2)
+            u0 = effective_psi_0 * pi / photon_in.wavelength()
+            a = pi / photon_in.wavelength() * SQ
+
+            complex_amplitude_s = (a * numpy.cos(a * s - a * T) - 1j * omega * numpy.sin(a * s - a* T))\
+                                  / (a * numpy.cos(a * T) + 1j * omega * numpy.sin(a * T))
+            complex_amplitude_s *= numpy.exp(1j * s * (omega + u0))
+
+            # pi polarization
+            effective_psi_h = numpy.conjugate(self.PsiH()) * cos(2 * self.braggAngle())
+            effective_psi_h_bar = numpy.conjugate(self.PsiHBar()) * cos(2 * self.braggAngle())
+            SQ = sqrt(guigay_b * effective_psi_h * effective_psi_h_bar + w ** 2)
+            u0 = effective_psi_0 * pi / photon_in.wavelength()
+            a = pi / photon_in.wavelength() * SQ
+
+            complex_amplitude_p = (a * numpy.cos(a * s - a * T) - 1j * omega * numpy.sin(a * s - a* T))\
+                                  / (a * numpy.cos(a * T) + 1j * omega * numpy.sin(a * T))
+            complex_amplitude_p *= numpy.exp(1j * s * (omega + u0))
+
+
+        elif self.geometryType() == LaueDiffraction():
+            if s_ratio is None:
+                s = T
+            else:
+                s = T * s_ratio
+                raise NotImplementedError()
+            # sigma polarization
+            effective_psi_h     = numpy.conjugate(self.PsiH())
+            effective_psi_h_bar = numpy.conjugate(self.PsiHBar())
+            SQ = sqrt(guigay_b * effective_psi_h * effective_psi_h_bar + w ** 2)
+            uh = effective_psi_h * pi / photon_in.wavelength()
+            u0 = effective_psi_0 * pi / photon_in.wavelength()
+            a = pi / photon_in.wavelength() * SQ
+
+            complex_amplitude_s = 1j * guigay_b * uh * sin(a * T) / a
+            complex_amplitude_s *= numpy.exp(1j * s * (omega + u0))
+
+            # pi polarization
+            effective_psi_h     = numpy.conjugate(self.PsiH()) * cos(2 * self.braggAngle())
+            effective_psi_h_bar = numpy.conjugate(self.PsiHBar()) * cos(2 * self.braggAngle())
+            SQ = sqrt(guigay_b * effective_psi_h * effective_psi_h_bar + w ** 2)
+            uh = effective_psi_h * pi / photon_in.wavelength()
+            u0 = effective_psi_0 * pi / photon_in.wavelength()
+            a = pi / photon_in.wavelength() * SQ
+
+            complex_amplitude_p = 1j * guigay_b * uh * sin(a * T) / a
+            complex_amplitude_p *= numpy.exp(1j * s * (omega + u0))
+
+        elif self.geometryType() == LaueTransmission():
+            if s_ratio is None:
+                s = T
+            else:
+                s = T * s_ratio
+                raise NotImplementedError()
+            # sigma polarization
+            effective_psi_h = numpy.conjugate(self.PsiH())
+            effective_psi_h_bar = numpy.conjugate(self.PsiHBar())
+            SQ = sqrt(guigay_b * effective_psi_h * effective_psi_h_bar + w ** 2)
+            a = pi / photon_in.wavelength() * SQ
+            u0 = effective_psi_0 * pi / photon_in.wavelength()
+
+            complex_amplitude_s = cos(a * T) - 1j * omega * sin(a * T) / a
+            complex_amplitude_s *= numpy.exp(1j * s * (omega + u0))
+
+            # pi polarization
+            effective_psi_h = numpy.conjugate(self.PsiH()) * cos(2 * self.braggAngle())
+            effective_psi_h_bar = numpy.conjugate(self.PsiHBar()) * cos(2 * self.braggAngle())
+            SQ = sqrt(guigay_b * effective_psi_h * effective_psi_h_bar + w ** 2)
+            a = pi / photon_in.wavelength() * SQ
+            u0 = effective_psi_0 * pi / photon_in.wavelength()
+
+            # pi polarization
+            complex_amplitude_p = cos(a * T) - 1j * omega * sin(a * T) / a
+            complex_amplitude_p *= numpy.exp(1j * s * (omega + u0))
+        else:
+            raise Exception
+
+
+
+        # Calculate complex amplitude for S and P polarization.
+        result["S"] = ComplexAmplitude(complex(complex_amplitude_s))
+        result["P"] = ComplexAmplitude(complex(complex_amplitude_p))
+
+        # Note division by |b| in intensity (thus sqrt(|b|) in amplitude)
+        # for power balance (see Zachariasen pag. 122)
+        #
+        # This factor only applies to diffracted beam, not to transmitted beams
+        # (see private communication M. Rio (ESRF) and J. Sutter (DLS))
+
+        if (self.geometryType() == BraggDiffraction() or
+                self.geometryType() == LaueDiffraction()):
+            result["S"].rescale(1.0 / sqrt(abs(guigay_b)))
+            result["P"].rescale(1.0 / sqrt(abs(guigay_b)))
+
+        # If debugging output is turned on.
+        if self.isDebug:
+            self._logMembers(guigay_b, zac_alpha, photon_in, photon_out, result)
+
+        # Returns the complex amplitudes.
+        return result
+
     def _logMembers(self, zac_b, zac_alpha, photon_in, photon_out, result):
         """
         Debug logs the member variables and other relevant partial results.
-        :param zac_b: Asymmetry ratio b as defined in Zachariasen [3-115].
+        :param zac_b: Asymmetry ratio b
         :param zac_alpha: Diffraction index difference of crystal fields.
         :param photon_in: Incoming photon.
         :param result: Resulting complex amplitudes of the diffraction/transmission.
         """
         self.logDebug("Bragg angle: %f degrees \n" % (self.braggAngle() * 180 / pi))
         self.logDebug("psi0: (%.14f , %.14f)" % (self.Psi0().real, self.Psi0().imag))
         self.logDebug("psiH: (%.14f , %.14f)" % (self.PsiH().real, self.PsiH().imag))
```

### Comparing `crystalpy-0.0.7/crystalpy/examples/PlotData1D.py` & `crystalpy-0.0.9/crystalpy/examples/PlotData1D.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/Si111.py` & `crystalpy-0.0.9/crystalpy/examples/Si111.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/Si111_energy_scan.py` & `crystalpy-0.0.9/crystalpy/examples/Si111_energy_scan.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/Si111_layered.py` & `crystalpy-0.0.9/crystalpy/examples/Si111_layered.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/Si111_simple.py` & `crystalpy-0.0.9/crystalpy/examples/Si111_simple.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/Si111_simple_xraylib_dabax_comparison.py` & `crystalpy-0.0.9/crystalpy/examples/Si111_simple_xraylib_dabax_comparison.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/Values.py` & `crystalpy-0.0.9/crystalpy/examples/Values.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/YB66.py` & `crystalpy-0.0.9/crystalpy/examples/YB66.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/check_against_xoppy_crystal.py` & `crystalpy-0.0.9/crystalpy/examples/check_against_xoppy_crystal.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/check_against_xoppy_crystal_including_shadow_proprocessor.py` & `crystalpy-0.0.9/crystalpy/examples/check_against_xoppy_crystal_including_shadow_proprocessor.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/check_structure_factor.py` & `crystalpy-0.0.9/crystalpy/examples/check_structure_factor.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/examples/main.py` & `crystalpy-0.0.9/crystalpy/examples/main.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/polarization/CrystalPhasePlate.py` & `crystalpy-0.0.9/crystalpy/polarization/CrystalPhasePlate.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/polarization/MuellerDiffraction.py` & `crystalpy-0.0.9/crystalpy/polarization/MuellerDiffraction.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/polarization/MuellerMatrix.py` & `crystalpy-0.0.9/crystalpy/polarization/MuellerMatrix.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/polarization/MuellerResult.py` & `crystalpy-0.0.9/crystalpy/polarization/MuellerResult.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/tests/PyCrystalTests.py` & `crystalpy-0.0.9/crystalpy/tests/PyCrystalTests.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/util/ComplexAmplitudePhoton.py` & `crystalpy-0.0.9/crystalpy/util/ComplexAmplitudePhoton.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/util/ComplexAmplitudePhotonBunch.py` & `crystalpy-0.0.9/crystalpy/util/ComplexAmplitudePhotonBunch.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/util/Photon.py` & `crystalpy-0.0.9/crystalpy/util/Photon.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/util/PhotonBunch.py` & `crystalpy-0.0.9/crystalpy/util/PhotonBunch.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/util/PolarizedPhoton.py` & `crystalpy-0.0.9/crystalpy/util/PolarizedPhoton.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/util/PolarizedPhotonBunch.py` & `crystalpy-0.0.9/crystalpy/util/PolarizedPhotonBunch.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/util/StokesVector.py` & `crystalpy-0.0.9/crystalpy/util/StokesVector.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy/util/Vector.py` & `crystalpy-0.0.9/crystalpy/util/Vector.py`

 * *Files identical despite different names*

### Comparing `crystalpy-0.0.7/crystalpy.egg-info/SOURCES.txt` & `crystalpy-0.0.9/crystalpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 crystalpy/diffraction/DiffractionSetupSweeps.py
 crystalpy/diffraction/GeometryType.py
 crystalpy/diffraction/PerfectCrystalDiffraction.py
 crystalpy/diffraction/__init__.py
 crystalpy/examples/PlotData1D.py
 crystalpy/examples/Si111.py
 crystalpy/examples/Si111_energy_scan.py
+crystalpy/examples/Si111_guigay.py
+crystalpy/examples/Si111_guigay_map_inside_crystal.py
 crystalpy/examples/Si111_layered.py
 crystalpy/examples/Si111_simple.py
 crystalpy/examples/Si111_simple_xraylib_dabax_comparison.py
 crystalpy/examples/Values.py
 crystalpy/examples/YB66.py
 crystalpy/examples/__init__.py
 crystalpy/examples/check_against_xoppy_crystal.py
```

### Comparing `crystalpy-0.0.7/setup.py` & `crystalpy-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # memorandum (for pypi)
 #
 # python setup.py sdist upload
 
 
 
 setup(name='crystalpy',
-      version='0.0.7',
+      version='0.0.9',
       description='Python crystal polarization calcution',
       author='Edoardo Cappelli, Mark Glass, Manuel Sanchez del Rio',
       author_email='srio@esrf.eu',
       url='https://github.com/edocappelli/crystalpy/',
       packages=['crystalpy',
                 'crystalpy.util',
                 'crystalpy.diffraction',
```

