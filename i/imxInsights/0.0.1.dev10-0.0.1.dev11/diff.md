# Comparing `tmp/imxinsights-0.0.1.dev10.tar.gz` & `tmp/imxinsights-0.0.1.dev11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imxinsights-0.0.1.dev10.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "imxinsights-0.0.1.dev11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `imxinsights-0.0.1.dev10.tar` & `imxinsights-0.0.1.dev11.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1708 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.github/workflows/package-build-and-deploy.yml
--rw-r--r--   0        0        0     1386 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.github/workflows/python-package-test-build.yml
--rw-r--r--   0        0        0     2700 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.gitignore
--rw-r--r--   0        0        0       47 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.idea/.gitignore
--rw-r--r--   0        0        0      491 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.idea/imxInsightsMonoRepo.iml
--rw-r--r--   0        0        0      817 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      208 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.idea/misc.xml
--rw-r--r--   0        0        0      290 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.idea/modules.xml
--rw-r--r--   0        0        0      180 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/.idea/vcs.xml
--rw-r--r--   0        0        0     1075 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/LICENSE.md
--rw-r--r--   0        0        0     1174 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/Makefile
--rw-r--r--   0        0        0     6382 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/README.md
--rw-r--r--   0        0        0      470 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs-overrides/main.html
--rw-r--r--   0        0        0       71 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/about.md
--rw-r--r--   0        0        0    12851 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/assets/img/ProRail_logo.svg
--rw-r--r--   0        0        0       59 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/contribute.md
--rw-r--r--   0        0        0     1749 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/examples/advanced/main.py
--rw-r--r--   0        0        0       11 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/examples/advanced/requirements.txt
--rw-r--r--   0        0        0      549 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/examples/diff/main.py
--rw-r--r--   0        0        0       11 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/examples/diff/requirements.txt
--rw-r--r--   0        0        0      702 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/examples/imx-example.md
--rw-r--r--   0        0        0     1299 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/examples/imx/main.py
--rw-r--r--   0        0        0       11 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/examples/imx/requirements.txt
--rw-r--r--   0        0        0      439 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/core/area.md
--rw-r--r--   0        0        0     1005 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/core/imx.md
--rw-r--r--   0        0        0     1328 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/core/imxObject.md
--rw-r--r--   0        0        0      441 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/core/imxPuic.md
--rw-r--r--   0        0        0      282 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/core/imxSituationRepo.md
--rw-r--r--   0        0        0      273 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/diff/change.md
--rw-r--r--   0        0        0      291 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/diff/compare.md
--rw-r--r--   0        0        0      421 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/diff/diff.md
--rw-r--r--   0        0        0      142 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/utils/general.md
--rw-r--r--   0        0        0      149 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/utils/shapely.md
--rw-r--r--   0        0        0      151 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/utils/shapelyGeojson.md
--rw-r--r--   0        0        0      146 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/imxInsights/utils/xml.md
--rw-r--r--   0        0        0       18 2023-06-15 13:33:43.436907 imxinsights-0.0.1.dev10/docs/index.md
--rw-r--r--   0        0        0  4713938 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/docs/notebooks/basic_use.ipynb
--rw-r--r--   0        0        0     2281 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/__init__.py
--rw-r--r--   0        0        0      840 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/custom_puic_config.yaml
--rw-r--r--   0        0        0        0 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/diff/__init__.py
--rw-r--r--   0        0        0      900 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/diff/areaStatusEnum.py
--rw-r--r--   0        0        0     4313 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/diff/change.py
--rw-r--r--   0        0        0    10668 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/diff/compair.py
--rw-r--r--   0        0        0      889 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/diff/diffStatusEnum.py
--rw-r--r--   0        0        0     9026 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/diff/imxDiff.py
--rw-r--r--   0        0        0        0 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/area/__init__.py
--rw-r--r--   0        0        0      657 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/area/area.py
--rw-r--r--   0        0        0      638 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/area/areaClassifiedTypeEnum.py
--rw-r--r--   0        0        0     5280 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/area/areaClassifier.py
--rw-r--r--   0        0        0     3100 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/area/imxProjectArea.py
--rw-r--r--   0        0        0     2427 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/imx.py
--rw-r--r--   0        0        0     3554 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/models/ImxRailConnectionInfo.py
--rw-r--r--   0        0        0        0 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/models/__init__.py
--rw-r--r--   0        0        0      753 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/models/imxEnums.py
--rw-r--r--   0        0        0     1002 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/models/imxGeometry.py
--rw-r--r--   0        0        0     9417 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/models/imxMetadata.py
--rw-r--r--   0        0        0     5657 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/models/imxPuic.py
--rw-r--r--   0        0        0      885 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/models/imxRelation.py
--rw-r--r--   0        0        0     3990 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/domain/models/imxSituations.py
--rw-r--r--   0        0        0        0 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/repo/__init__.py
--rw-r--r--   0        0        0    18122 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/repo/imxRepo.py
--rw-r--r--   0        0        0        0 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/repo/tree/__init__.py
--rw-r--r--   0        0        0     1199 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/repo/tree/imxTopoTreeObject.py
--rw-r--r--   0        0        0     7924 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/repo/tree/imxTreeObject.py
--rw-r--r--   0        0        0     4132 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/repo/tree/objectTree.py
--rw-r--r--   0        0        0       56 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/utils/__init__.py
--rw-r--r--   0        0        0     3395 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/utils/helpers.py
--rw-r--r--   0        0        0     1308 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/utils/log.py
--rw-r--r--   0        0        0     5778 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/utils/shapely_geojson.py
--rw-r--r--   0        0        0     3808 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/utils/shapely_helpers.py
--rw-r--r--   0        0        0     3620 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/imxInsights/utils/xml_helpers.py
--rw-r--r--   0        0        0     2470 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/mkdocs.yml
--rw-r--r--   0        0        0     1797 2023-06-15 13:33:43.456907 imxinsights-0.0.1.dev10/pyproject.toml
--rw-r--r--   0        0        0  7366031 2023-06-15 13:33:43.476908 imxinsights-0.0.1.dev10/sample_data/Groningen_verrijkt.xml
--rw-r--r--   0        0        0 10387299 2023-06-15 13:33:43.508908 imxinsights-0.0.1.dev10/sample_data/Hanzelijn_verrijkt_latest.xml
--rw-r--r--   0        0        0  7917973 2023-06-15 13:33:43.552908 imxinsights-0.0.1.dev10/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml
--rw-r--r--   0        0        0 15685770 2023-06-15 13:33:43.600909 imxinsights-0.0.1.dev10/sample_data/O_RVTOv2.0_20230602145547.xml
--rw-r--r--   0        0        0  4762050 2023-06-15 13:33:43.624909 imxinsights-0.0.1.dev10/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml
--rw-r--r--   0        0        0 15304541 2023-06-15 13:33:43.696910 imxinsights-0.0.1.dev10/sample_data/U_totaal ENL_20230501_compleet_imx500.xml
--rw-r--r--   0        0        0  1561875 2023-06-15 13:33:43.700910 imxinsights-0.0.1.dev10/sample_data/leeuwarden_verrijkt.xml
--rw-r--r--   0        0        0      332 2023-06-15 13:33:43.700910 imxinsights-0.0.1.dev10/settings.json
--rw-r--r--   0        0        0      671 2023-06-15 13:33:43.700910 imxinsights-0.0.1.dev10/setup.cfg
--rw-r--r--   0        0        0       99 2023-06-15 13:33:43.700910 imxinsights-0.0.1.dev10/test_build.py
--rw-r--r--   0        0        0        0 2023-06-15 13:33:43.700910 imxinsights-0.0.1.dev10/tests/__init__.py
--rw-r--r--   0        0        0      133 2023-06-15 13:33:43.700910 imxinsights-0.0.1.dev10/tests/conftest.py
--rw-r--r--   0        0        0      616 2023-06-15 13:33:43.704910 imxinsights-0.0.1.dev10/tests/fixtures/files.py
--rw-r--r--   0        0        0      182 2023-06-15 13:33:43.704910 imxinsights-0.0.1.dev10/tests/fixtures/imx_files.py
--rw-r--r--   0        0        0      811 2023-06-15 13:33:43.704910 imxinsights-0.0.1.dev10/tests/helpers.py
--rw-r--r--   0        0        0     5886 2023-06-15 13:33:43.704910 imxinsights-0.0.1.dev10/tests/test_imx.py
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev10/setup.py
--rw-r--r--   0        0        0     8035 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev10/PKG-INFO
+-rw-r--r--   0        0        0     1708 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.github/workflows/package-build-and-deploy.yml
+-rw-r--r--   0        0        0     1386 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.github/workflows/python-package-test-build.yml
+-rw-r--r--   0        0        0     2700 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.gitignore
+-rw-r--r--   0        0        0       47 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/.gitignore
+-rw-r--r--   0        0        0      491 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/imxInsightsMonoRepo.iml
+-rw-r--r--   0        0        0      817 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      208 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/misc.xml
+-rw-r--r--   0        0        0      290 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/vcs.xml
+-rw-r--r--   0        0        0     1075 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/LICENSE.md
+-rw-r--r--   0        0        0     1174 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/Makefile
+-rw-r--r--   0        0        0     6378 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/README.md
+-rw-r--r--   0        0        0      470 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs-overrides/main.html
+-rw-r--r--   0        0        0       71 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/about.md
+-rw-r--r--   0        0        0    12851 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/assets/img/ProRail_logo.svg
+-rw-r--r--   0        0        0       59 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/contribute.md
+-rw-r--r--   0        0        0     1749 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/advanced/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/advanced/requirements.txt
+-rw-r--r--   0        0        0      549 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/diff/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/diff/requirements.txt
+-rw-r--r--   0        0        0      702 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/imx-example.md
+-rw-r--r--   0        0        0     1299 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/imx/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/imx/requirements.txt
+-rw-r--r--   0        0        0      439 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/area.md
+-rw-r--r--   0        0        0     1005 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/imx.md
+-rw-r--r--   0        0        0     1328 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/imxObject.md
+-rw-r--r--   0        0        0      441 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/imxPuic.md
+-rw-r--r--   0        0        0      282 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/imxSituationRepo.md
+-rw-r--r--   0        0        0      273 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/diff/change.md
+-rw-r--r--   0        0        0      291 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/diff/compare.md
+-rw-r--r--   0        0        0      421 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/diff/diff.md
+-rw-r--r--   0        0        0      142 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/utils/general.md
+-rw-r--r--   0        0        0      149 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/utils/shapely.md
+-rw-r--r--   0        0        0      151 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/utils/shapelyGeojson.md
+-rw-r--r--   0        0        0      146 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/utils/xml.md
+-rw-r--r--   0        0        0       18 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/index.md
+-rw-r--r--   0        0        0  4713938 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/docs/notebooks/basic_use.ipynb
+-rw-r--r--   0        0        0     2281 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/__init__.py
+-rw-r--r--   0        0        0      840 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/custom_puic_config.yaml
+-rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/areaStatusEnum.py
+-rw-r--r--   0        0        0     4313 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/change.py
+-rw-r--r--   0        0        0    10668 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/compair.py
+-rw-r--r--   0        0        0      889 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/diffStatusEnum.py
+-rw-r--r--   0        0        0     9026 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/imxDiff.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/__init__.py
+-rw-r--r--   0        0        0      657 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/area.py
+-rw-r--r--   0        0        0      638 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/areaClassifiedTypeEnum.py
+-rw-r--r--   0        0        0     5280 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/areaClassifier.py
+-rw-r--r--   0        0        0     3100 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/imxProjectArea.py
+-rw-r--r--   0        0        0     5980 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/imx.py
+-rw-r--r--   0        0        0     3554 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/ImxRailConnectionInfo.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxEnums.py
+-rw-r--r--   0        0        0     1002 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxGeometry.py
+-rw-r--r--   0        0        0     9417 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxMetadata.py
+-rw-r--r--   0        0        0     5657 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxPuic.py
+-rw-r--r--   0        0        0      885 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxRelation.py
+-rw-r--r--   0        0        0     3990 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxSituations.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/__init__.py
+-rw-r--r--   0        0        0    19150 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/imxRepo.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/tree/__init__.py
+-rw-r--r--   0        0        0     1199 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/tree/imxTopoTreeObject.py
+-rw-r--r--   0        0        0     7924 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/tree/imxTreeObject.py
+-rw-r--r--   0        0        0     4132 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/tree/objectTree.py
+-rw-r--r--   0        0        0       56 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/__init__.py
+-rw-r--r--   0        0        0     3653 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/helpers.py
+-rw-r--r--   0        0        0     1308 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/log.py
+-rw-r--r--   0        0        0     5778 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/shapely_geojson.py
+-rw-r--r--   0        0        0     3808 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/shapely_helpers.py
+-rw-r--r--   0        0        0     3620 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/xml_helpers.py
+-rw-r--r--   0        0        0     2470 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/mkdocs.yml
+-rw-r--r--   0        0        0     1798 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/pyproject.toml
+-rw-r--r--   0        0        0  7366031 2023-06-21 10:18:11.657553 imxinsights-0.0.1.dev11/sample_data/Groningen_verrijkt.xml
+-rw-r--r--   0        0        0 10387299 2023-06-21 10:18:11.685553 imxinsights-0.0.1.dev11/sample_data/Hanzelijn_verrijkt_latest.xml
+-rw-r--r--   0        0        0  7917973 2023-06-21 10:18:11.737553 imxinsights-0.0.1.dev11/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml
+-rw-r--r--   0        0        0 15685770 2023-06-21 10:18:11.785554 imxinsights-0.0.1.dev11/sample_data/O_RVTOv2.0_20230602145547.xml
+-rw-r--r--   0        0        0  4762050 2023-06-21 10:18:11.809553 imxinsights-0.0.1.dev11/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml
+-rw-r--r--   0        0        0 15304541 2023-06-21 10:18:11.889554 imxinsights-0.0.1.dev11/sample_data/U_totaal ENL_20230501_compleet_imx500.xml
+-rw-r--r--   0        0        0  1561875 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/sample_data/leeuwarden_verrijkt.xml
+-rw-r--r--   0        0        0      332 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/settings.json
+-rw-r--r--   0        0        0      671 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/setup.cfg
+-rw-r--r--   0        0        0       99 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/test_build.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/conftest.py
+-rw-r--r--   0        0        0      616 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/fixtures/files.py
+-rw-r--r--   0        0        0      182 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/fixtures/imx_files.py
+-rw-r--r--   0        0        0      811 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/helpers.py
+-rw-r--r--   0        0        0     6497 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/test_imx.py
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev11/setup.py
+-rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev11/PKG-INFO
```

### Comparing `imxinsights-0.0.1.dev10/.github/workflows/package-build-and-deploy.yml` & `imxinsights-0.0.1.dev11/.github/workflows/package-build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/.github/workflows/python-package-test-build.yml` & `imxinsights-0.0.1.dev11/.github/workflows/python-package-test-build.yml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/.gitignore` & `imxinsights-0.0.1.dev11/.gitignore`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/.idea/inspectionProfiles/Project_Default.xml` & `imxinsights-0.0.1.dev11/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/LICENSE.md` & `imxinsights-0.0.1.dev11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/Makefile` & `imxinsights-0.0.1.dev11/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 	flake8 ./imxInsights ./tests
 
 typecheck:
 	mypy imxInsights/ tests/
 
 # todo: make sure in production covar is at least 90%
 test:
-	pytest --cov=imxInsights/ --cov-report=term-missing --cov-fail-under=68
+	pytest --cov=imxInsights/ --cov-report=term-missing --cov-fail-under=70
 
 bumpversion-major:
 	bumpversion major
 
 bumpversion-minor:
 	bumpversion minor
```

### Comparing `imxinsights-0.0.1.dev10/README.md` & `imxinsights-0.0.1.dev11/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 pandas_df = imx.project.new_situation.get_pandas_df("Signal")
 ```
 
 For more code samples and snippets in the example section / folder and use the api reference for exploration.
 
 ## Roadmap
 - [ ] imx diff
-- [ ] ~~pypi release 0.0.1~~
-- [ ] documentation and webpage
+- [X] pypi release 0.0.1
+- [X] documentation and webpage
 - [ ] 100% code coverage 
 - [ ] release 0.1.0
 - [ ] imx map
 - [ ] imx report
 - [ ] imx graph
 
 --8<-- [end:main]
```

### Comparing `imxinsights-0.0.1.dev10/docs/assets/img/ProRail_logo.svg` & `imxinsights-0.0.1.dev11/docs/assets/img/ProRail_logo.svg`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/docs/examples/advanced/main.py` & `imxinsights-0.0.1.dev11/docs/examples/advanced/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/docs/examples/diff/main.py` & `imxinsights-0.0.1.dev11/docs/examples/diff/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/docs/examples/imx-example.md` & `imxinsights-0.0.1.dev11/docs/examples/imx-example.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/docs/examples/imx/main.py` & `imxinsights-0.0.1.dev11/docs/examples/imx/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/docs/imxInsights/core/imx.md` & `imxinsights-0.0.1.dev11/docs/imxInsights/core/imx.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/docs/imxInsights/core/imxObject.md` & `imxinsights-0.0.1.dev11/docs/imxInsights/core/imxObject.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/docs/notebooks/basic_use.ipynb` & `imxinsights-0.0.1.dev11/docs/notebooks/basic_use.ipynb`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/__init__.py` & `imxinsights-0.0.1.dev11/imxInsights/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1-dev10"
+__version__ = "0.0.1-dev11"
 
 
 from .diff.areaStatusEnum import AreaStatusEnum
 from .diff.change import Change, ChangeList
 from .diff.compair import ImxObjectCompare, ImxPropertyCompare
 from .diff.diffStatusEnum import DiffStatusEnum
 from .diff.imxDiff import ImxDiff
```

### Comparing `imxinsights-0.0.1.dev10/imxInsights/custom_puic_config.yaml` & `imxinsights-0.0.1.dev11/imxInsights/custom_puic_config.yaml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/diff/areaStatusEnum.py` & `imxinsights-0.0.1.dev11/imxInsights/diff/areaStatusEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/diff/change.py` & `imxinsights-0.0.1.dev11/imxInsights/diff/change.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/diff/compair.py` & `imxinsights-0.0.1.dev11/imxInsights/diff/compair.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/diff/diffStatusEnum.py` & `imxinsights-0.0.1.dev11/imxInsights/diff/diffStatusEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/diff/imxDiff.py` & `imxinsights-0.0.1.dev11/imxInsights/diff/imxDiff.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/area/area.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/area/area.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/area/areaClassifiedTypeEnum.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/area/areaClassifiedTypeEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/area/areaClassifier.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/area/areaClassifier.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/area/imxProjectArea.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/area/imxProjectArea.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/models/ImxRailConnectionInfo.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/models/ImxRailConnectionInfo.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/models/imxEnums.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxEnums.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/models/imxGeometry.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxGeometry.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/models/imxMetadata.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxMetadata.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/models/imxPuic.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxPuic.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/models/imxRelation.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxRelation.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/domain/models/imxSituations.py` & `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxSituations.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/repo/imxRepo.py` & `imxinsights-0.0.1.dev11/imxInsights/repo/imxRepo.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 from imxInsights.domain.models.imxEnums import AreaNameEnum
 from imxInsights.domain.models.imxGeometry import ImxGeometry
 from imxInsights.domain.models.imxRelation import ImxRelation
 from imxInsights.repo.tree.imxTreeObject import ImxObject
 from imxInsights.repo.tree.objectTree import ObjectTree
 from imxInsights.utils.log import logger
+from imxInsights.utils.shapely_geojson import GeoJsonFeature, GeoJsonFeatureCollection
 from imxInsights.utils.shapely_helpers import (
+    ShapelyTransform,
     gml_linestring_to_shapely,
     gml_point_to_shapely,
     gml_polygon_to_shapely,
     reverse_line,
 )
 from imxInsights.utils.xml_helpers import NS_GML, NS_IMSPOOR, find_coordinates, trim_tag
 
@@ -404,12 +406,33 @@
                 out_dict[imx_type] = self.get_pandas_df(imx_type)
 
         for imx_path in self.get_all_paths():
             out_dict[imx_path] = self.get_pandas_df(imx_path)
 
         return out_dict
 
-    def get_geojson(self, object_type_or_path: str = None, as_string: bool = True) -> str:
-        pass
+    def get_geojson(self, object_type_or_path: str, in_rd: bool = False) -> GeoJsonFeatureCollection:
+        if "." in object_type_or_path:
+            records = self.get_by_paths([object_type_or_path])
+        else:
+            records = self.get_by_types([object_type_or_path])
+
+        if in_rd:
+            features = [GeoJsonFeature(properties=record.properties, geometry_list=[record.shapely]) for record in records]
+        else:
+            features = [
+                GeoJsonFeature(properties=record.properties, geometry_list=[ShapelyTransform.rd_to_wgs(record.shapely)]) for record in records
+            ]
+
+        feature_collection = GeoJsonFeatureCollection(features)
+        return feature_collection
+
+    def get_geojson_dict(self, key_based_on_type: bool = False, in_rd: bool = False) -> Dict[str, GeoJsonFeatureCollection]:
+        out_dict = {}
+        if key_based_on_type:
+            for imx_type in self.get_all_types():
+                out_dict[imx_type] = self.get_geojson(imx_type)
 
-    def get_geojson_dict(self, key_based_on_type: bool = None, as_string: bool = True) -> Dict[str, str]:
-        pass
+        for imx_path in self.get_all_paths():
+            out_dict[imx_path] = self.get_geojson(imx_path)
+
+        return out_dict
```

### Comparing `imxinsights-0.0.1.dev10/imxInsights/repo/tree/imxTopoTreeObject.py` & `imxinsights-0.0.1.dev11/imxInsights/repo/tree/imxTopoTreeObject.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/repo/tree/imxTreeObject.py` & `imxinsights-0.0.1.dev11/imxInsights/repo/tree/imxTreeObject.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/repo/tree/objectTree.py` & `imxinsights-0.0.1.dev11/imxInsights/repo/tree/objectTree.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/utils/helpers.py` & `imxinsights-0.0.1.dev11/imxInsights/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import os
 from typing import Any, Dict, List, Optional
 
 from ruamel.yaml import YAML
 
 
 def get_yaml_dict(file_path):
@@ -98,7 +99,17 @@
         # Add index for each child if >1 and recurse.
         for i, child in enumerate(remaining):
             child_prefix = f"{new_prefix}{i}{sep}" if len(remaining) > 1 else new_prefix
             flattened = flatten_dict(child, skip_key=skip_key, prefix=child_prefix, sep=sep)
             result = result | flattened
 
     return result
+
+
+def sha256sum(filename):
+    h = hashlib.sha256()
+    b = bytearray(128 * 1024)
+    mv = memoryview(b)
+    with open(filename, "rb", buffering=0) as f:
+        while n := f.readinto(mv):
+            h.update(mv[:n])
+    return h.hexdigest()
```

### Comparing `imxinsights-0.0.1.dev10/imxInsights/utils/log.py` & `imxinsights-0.0.1.dev11/imxInsights/utils/log.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/utils/shapely_geojson.py` & `imxinsights-0.0.1.dev11/imxInsights/utils/shapely_geojson.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/utils/shapely_helpers.py` & `imxinsights-0.0.1.dev11/imxInsights/utils/shapely_helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/imxInsights/utils/xml_helpers.py` & `imxinsights-0.0.1.dev11/imxInsights/utils/xml_helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/mkdocs.yml` & `imxinsights-0.0.1.dev11/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/pyproject.toml` & `imxinsights-0.0.1.dev11/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 ]
 
 jupyter = [
     "jupyterlab",
     "pygwalker"
 ]
 
+
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [tool.isort]
 profile = "black"
 skip = []
```

### Comparing `imxinsights-0.0.1.dev10/sample_data/Groningen_verrijkt.xml` & `imxinsights-0.0.1.dev11/sample_data/Groningen_verrijkt.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/sample_data/Hanzelijn_verrijkt_latest.xml` & `imxinsights-0.0.1.dev11/sample_data/Hanzelijn_verrijkt_latest.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml` & `imxinsights-0.0.1.dev11/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/sample_data/O_RVTOv2.0_20230602145547.xml` & `imxinsights-0.0.1.dev11/sample_data/O_RVTOv2.0_20230602145547.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml` & `imxinsights-0.0.1.dev11/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/sample_data/U_totaal ENL_20230501_compleet_imx500.xml` & `imxinsights-0.0.1.dev11/sample_data/U_totaal ENL_20230501_compleet_imx500.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/sample_data/leeuwarden_verrijkt.xml` & `imxinsights-0.0.1.dev11/sample_data/leeuwarden_verrijkt.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/setup.cfg` & `imxinsights-0.0.1.dev11/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [bumpversion]
 commit = True
 tag = True
-current_version = 0.0.1-dev10
+current_version = 0.0.1-dev11
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>.*)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
 
 [bumpversion:part:release]
 optional_value = gamma
```

### Comparing `imxinsights-0.0.1.dev10/tests/fixtures/files.py` & `imxinsights-0.0.1.dev11/tests/fixtures/files.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/tests/helpers.py` & `imxinsights-0.0.1.dev11/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev10/tests/test_imx.py` & `imxinsights-0.0.1.dev11/tests/test_imx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,32 @@
+from pathlib import Path
+
 import pytest
 
+from imxInsights import GeoJsonFeatureCollection, ImxSituationsEnum
+
 # from imxInsights.diff.imxDiff import ImxDiff
 from imxInsights.domain.imx import Imx
 
 
 @pytest.mark.slow
 def test_imx_parse_project_v500(get_imx_project_test_file_path, tmp_path: str):
     imx = Imx(get_imx_project_test_file_path)
+
+    imx.generate_population_excel("tester.xlsx", ImxSituationsEnum.InitialSituation)
+    file_path = Path("tester.xlsx")
+    assert file_path.exists(), "file should exist"
+    file_path.unlink()
+
+    signals_geojson = imx.project.initial_situation.get_geojson(object_type_or_path="Signal")
+    assert isinstance(signals_geojson, GeoJsonFeatureCollection), "should return feature collection"
+
+    geojson = imx.project.initial_situation.get_geojson_dict()
+    assert isinstance(geojson, dict), "should return dict"
+
     assert imx.imx_version == "5.0.0", "imx version should be 5.0.0"
 
     # diff = ImxDiff(imx.project.initial_situation, imx.project.new_situation)
     # dict_of_df_of_all_types = diff.pandas_dataframe_dict()
     # df_micro_nodes = diff.pandas_dataframe("MicroNode", geometry=False)
     # df_signals = diff.pandas_dataframe("Signal", geometry=True)
     # df_rail_con = diff.pandas_dataframe("RailConnection", geometry=True)
```

### Comparing `imxinsights-0.0.1.dev10/setup.py` & `imxinsights-0.0.1.dev11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
          'mkdocs-material',
          'mkdocs-mermaid2-plugin',
          'mkdocstrings[crystal, python]>=0.18',
          'pymdown-extensions'],
  'jupyter': ['jupyterlab', 'pygwalker']}
 
 setup(name='imxInsights',
-      version='0.0.1.dev10',
+      version='0.0.1.dev11',
       description='python imx insights module to get information from imx files',
       author=None,
       author_email='Hzd <Hazedd@users.noreply.github.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `imxinsights-0.0.1.dev10/PKG-INFO` & `imxinsights-0.0.1.dev11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imxInsights
-Version: 0.0.1.dev10
+Version: 0.0.1.dev11
 Summary: python imx insights module to get information from imx files
 Author-email: Hzd <Hazedd@users.noreply.github.com>
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3.10
@@ -107,16 +107,16 @@
 pandas_df = imx.project.new_situation.get_pandas_df("Signal")
 ```
 
 For more code samples and snippets in the example section / folder and use the api reference for exploration.
 
 ## Roadmap
 - [ ] imx diff
-- [ ] ~~pypi release 0.0.1~~
-- [ ] documentation and webpage
+- [X] pypi release 0.0.1
+- [X] documentation and webpage
 - [ ] 100% code coverage 
 - [ ] release 0.1.0
 - [ ] imx map
 - [ ] imx report
 - [ ] imx graph
 
 --8<-- [end:main]
```

