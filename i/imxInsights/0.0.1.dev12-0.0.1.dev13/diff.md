# Comparing `tmp/imxinsights-0.0.1.dev12.tar.gz` & `tmp/imxinsights-0.0.1.dev13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imxinsights-0.0.1.dev12.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "imxinsights-0.0.1.dev13.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `imxinsights-0.0.1.dev12.tar` & `imxinsights-0.0.1.dev13.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1708 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.github/workflows/package-build-and-deploy.yml
--rw-r--r--   0        0        0     1417 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.github/workflows/python-package-test-build.yml
--rw-r--r--   0        0        0     2700 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.gitignore
--rw-r--r--   0        0        0       47 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/.gitignore
--rw-r--r--   0        0        0      491 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/imxInsightsMonoRepo.iml
--rw-r--r--   0        0        0      817 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      208 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/misc.xml
--rw-r--r--   0        0        0      290 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/modules.xml
--rw-r--r--   0        0        0      180 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/vcs.xml
--rw-r--r--   0        0        0     1075 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/LICENSE.md
--rw-r--r--   0        0        0     1174 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/Makefile
--rw-r--r--   0        0        0     6378 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/README.md
--rw-r--r--   0        0        0      470 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs-overrides/main.html
--rw-r--r--   0        0        0       71 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/about.md
--rw-r--r--   0        0        0    12851 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/assets/img/ProRail_logo.svg
--rw-r--r--   0        0        0       59 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/contribute.md
--rw-r--r--   0        0        0     1749 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/advanced/main.py
--rw-r--r--   0        0        0       11 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/advanced/requirements.txt
--rw-r--r--   0        0        0      549 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/diff/main.py
--rw-r--r--   0        0        0       11 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/diff/requirements.txt
--rw-r--r--   0        0        0      702 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/imx-example.md
--rw-r--r--   0        0        0     1299 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/imx/main.py
--rw-r--r--   0        0        0       11 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/imx/requirements.txt
--rw-r--r--   0        0        0      439 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/area.md
--rw-r--r--   0        0        0     1005 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/imx.md
--rw-r--r--   0        0        0     1328 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/imxObject.md
--rw-r--r--   0        0        0      441 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/imxPuic.md
--rw-r--r--   0        0        0      282 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/imxSituationRepo.md
--rw-r--r--   0        0        0      273 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/diff/change.md
--rw-r--r--   0        0        0      291 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/diff/compare.md
--rw-r--r--   0        0        0      421 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/diff/diff.md
--rw-r--r--   0        0        0      142 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/utils/general.md
--rw-r--r--   0        0        0      149 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/utils/shapely.md
--rw-r--r--   0        0        0      151 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/utils/shapelyGeojson.md
--rw-r--r--   0        0        0      146 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/utils/xml.md
--rw-r--r--   0        0        0       18 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/index.md
--rw-r--r--   0        0        0  4713938 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/docs/notebooks/basic_use.ipynb
--rw-r--r--   0        0        0     2281 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/imxInsights/__init__.py
--rw-r--r--   0        0        0      840 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/imxInsights/custom_puic_config.yaml
--rw-r--r--   0        0        0        0 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/imxInsights/diff/__init__.py
--rw-r--r--   0        0        0      900 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/imxInsights/diff/areaStatusEnum.py
--rw-r--r--   0        0        0     4313 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/diff/change.py
--rw-r--r--   0        0        0    10668 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/diff/compair.py
--rw-r--r--   0        0        0      889 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/diff/diffStatusEnum.py
--rw-r--r--   0        0        0     9026 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/diff/imxDiff.py
--rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/__init__.py
--rw-r--r--   0        0        0      657 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/area.py
--rw-r--r--   0        0        0      638 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/areaClassifiedTypeEnum.py
--rw-r--r--   0        0        0     5280 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/areaClassifier.py
--rw-r--r--   0        0        0     3100 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/imxProjectArea.py
--rw-r--r--   0        0        0     6905 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/imx.py
--rw-r--r--   0        0        0     3554 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/ImxRailConnectionInfo.py
--rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/__init__.py
--rw-r--r--   0        0        0      753 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxEnums.py
--rw-r--r--   0        0        0     1002 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxGeometry.py
--rw-r--r--   0        0        0     9417 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxMetadata.py
--rw-r--r--   0        0        0     5657 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxPuic.py
--rw-r--r--   0        0        0      885 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxRelation.py
--rw-r--r--   0        0        0     3990 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxSituations.py
--rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/__init__.py
--rw-r--r--   0        0        0    19150 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/imxRepo.py
--rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/tree/__init__.py
--rw-r--r--   0        0        0     1199 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/tree/imxTopoTreeObject.py
--rw-r--r--   0        0        0     7924 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/tree/imxTreeObject.py
--rw-r--r--   0        0        0     4132 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/tree/objectTree.py
--rw-r--r--   0        0        0       56 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/__init__.py
--rw-r--r--   0        0        0     3653 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/helpers.py
--rw-r--r--   0        0        0     1308 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/log.py
--rw-r--r--   0        0        0     5778 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/shapely_geojson.py
--rw-r--r--   0        0        0     3808 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/shapely_helpers.py
--rw-r--r--   0        0        0     3620 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/xml_helpers.py
--rw-r--r--   0        0        0     2470 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/mkdocs.yml
--rw-r--r--   0        0        0     1798 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/pyproject.toml
--rw-r--r--   0        0        0  7366031 2023-06-21 15:08:22.880446 imxinsights-0.0.1.dev12/sample_data/Groningen_verrijkt.xml
--rw-r--r--   0        0        0 10387299 2023-06-21 15:08:22.912446 imxinsights-0.0.1.dev12/sample_data/Hanzelijn_verrijkt_latest.xml
--rw-r--r--   0        0        0  7917973 2023-06-21 15:08:22.960447 imxinsights-0.0.1.dev12/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml
--rw-r--r--   0        0        0 15685770 2023-06-21 15:08:23.004447 imxinsights-0.0.1.dev12/sample_data/O_RVTOv2.0_20230602145547.xml
--rw-r--r--   0        0        0  4762050 2023-06-21 15:08:23.028448 imxinsights-0.0.1.dev12/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml
--rw-r--r--   0        0        0 15304541 2023-06-21 15:08:23.104449 imxinsights-0.0.1.dev12/sample_data/U_totaal ENL_20230501_compleet_imx500.xml
--rw-r--r--   0        0        0  1561875 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/sample_data/leeuwarden_verrijkt.xml
--rw-r--r--   0        0        0      332 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/settings.json
--rw-r--r--   0        0        0      671 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/setup.cfg
--rw-r--r--   0        0        0       99 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/test_build.py
--rw-r--r--   0        0        0        0 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/__init__.py
--rw-r--r--   0        0        0      133 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/conftest.py
--rw-r--r--   0        0        0      616 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/fixtures/files.py
--rw-r--r--   0        0        0      182 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/fixtures/imx_files.py
--rw-r--r--   0        0        0      811 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/helpers.py
--rw-r--r--   0        0        0     6493 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/test_imx.py
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev12/setup.py
--rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev12/PKG-INFO
+-rw-r--r--   0        0        0     1708 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.github/workflows/package-build-and-deploy.yml
+-rw-r--r--   0        0        0     1417 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.github/workflows/python-package-test-build.yml
+-rw-r--r--   0        0        0     2700 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.gitignore
+-rw-r--r--   0        0        0       47 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.idea/.gitignore
+-rw-r--r--   0        0        0      491 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.idea/imxInsightsMonoRepo.iml
+-rw-r--r--   0        0        0      817 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      208 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.idea/misc.xml
+-rw-r--r--   0        0        0      290 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/.idea/vcs.xml
+-rw-r--r--   0        0        0     1075 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/LICENSE.md
+-rw-r--r--   0        0        0     1174 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/Makefile
+-rw-r--r--   0        0        0     6378 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/README.md
+-rw-r--r--   0        0        0      470 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs-overrides/main.html
+-rw-r--r--   0        0        0       71 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/about.md
+-rw-r--r--   0        0        0    12851 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/assets/img/ProRail_logo.svg
+-rw-r--r--   0        0        0       59 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/contribute.md
+-rw-r--r--   0        0        0     1749 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/examples/advanced/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/examples/advanced/requirements.txt
+-rw-r--r--   0        0        0      549 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/examples/diff/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/examples/diff/requirements.txt
+-rw-r--r--   0        0        0      702 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/examples/imx-example.md
+-rw-r--r--   0        0        0     1299 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/examples/imx/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/examples/imx/requirements.txt
+-rw-r--r--   0        0        0      439 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/core/area.md
+-rw-r--r--   0        0        0     1005 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/core/imx.md
+-rw-r--r--   0        0        0     1328 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/core/imxObject.md
+-rw-r--r--   0        0        0      441 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/core/imxPuic.md
+-rw-r--r--   0        0        0      282 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/core/imxSituationRepo.md
+-rw-r--r--   0        0        0      273 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/diff/change.md
+-rw-r--r--   0        0        0      291 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/diff/compare.md
+-rw-r--r--   0        0        0      421 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/diff/diff.md
+-rw-r--r--   0        0        0      142 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/utils/general.md
+-rw-r--r--   0        0        0      149 2023-06-21 17:43:04.444847 imxinsights-0.0.1.dev13/docs/imxInsights/utils/shapely.md
+-rw-r--r--   0        0        0      151 2023-06-21 17:43:04.448847 imxinsights-0.0.1.dev13/docs/imxInsights/utils/shapelyGeojson.md
+-rw-r--r--   0        0        0      146 2023-06-21 17:43:04.448847 imxinsights-0.0.1.dev13/docs/imxInsights/utils/xml.md
+-rw-r--r--   0        0        0       18 2023-06-21 17:43:04.448847 imxinsights-0.0.1.dev13/docs/index.md
+-rw-r--r--   0        0        0  4713938 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/docs/notebooks/basic_use.ipynb
+-rw-r--r--   0        0        0     2281 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/__init__.py
+-rw-r--r--   0        0        0      840 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/custom_puic_config.yaml
+-rw-r--r--   0        0        0        0 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/diff/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/diff/areaStatusEnum.py
+-rw-r--r--   0        0        0     4313 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/diff/change.py
+-rw-r--r--   0        0        0    10668 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/diff/compair.py
+-rw-r--r--   0        0        0      889 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/diff/diffStatusEnum.py
+-rw-r--r--   0        0        0     9657 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/diff/imxDiff.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/area/__init__.py
+-rw-r--r--   0        0        0      657 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/area/area.py
+-rw-r--r--   0        0        0      638 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/area/areaClassifiedTypeEnum.py
+-rw-r--r--   0        0        0     5280 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/area/areaClassifier.py
+-rw-r--r--   0        0        0     3100 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/area/imxProjectArea.py
+-rw-r--r--   0        0        0     6905 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/imx.py
+-rw-r--r--   0        0        0     3554 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/models/ImxRailConnectionInfo.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/models/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/models/imxEnums.py
+-rw-r--r--   0        0        0     1002 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/models/imxGeometry.py
+-rw-r--r--   0        0        0     9417 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/models/imxMetadata.py
+-rw-r--r--   0        0        0     5657 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/models/imxPuic.py
+-rw-r--r--   0        0        0      885 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/models/imxRelation.py
+-rw-r--r--   0        0        0     3990 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/domain/models/imxSituations.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/repo/__init__.py
+-rw-r--r--   0        0        0    19150 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/repo/imxRepo.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/repo/tree/__init__.py
+-rw-r--r--   0        0        0     1199 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/repo/tree/imxTopoTreeObject.py
+-rw-r--r--   0        0        0     7924 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/repo/tree/imxTreeObject.py
+-rw-r--r--   0        0        0     4132 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/repo/tree/objectTree.py
+-rw-r--r--   0        0        0       56 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/utils/__init__.py
+-rw-r--r--   0        0        0     3653 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/utils/helpers.py
+-rw-r--r--   0        0        0     1308 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/utils/log.py
+-rw-r--r--   0        0        0     5778 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/utils/shapely_geojson.py
+-rw-r--r--   0        0        0     3808 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/utils/shapely_helpers.py
+-rw-r--r--   0        0        0     3620 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/imxInsights/utils/xml_helpers.py
+-rw-r--r--   0        0        0     2470 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/mkdocs.yml
+-rw-r--r--   0        0        0     1798 2023-06-21 17:43:04.464847 imxinsights-0.0.1.dev13/pyproject.toml
+-rw-r--r--   0        0        0  7366031 2023-06-21 17:43:04.484847 imxinsights-0.0.1.dev13/sample_data/Groningen_verrijkt.xml
+-rw-r--r--   0        0        0 10387299 2023-06-21 17:43:04.516847 imxinsights-0.0.1.dev13/sample_data/Hanzelijn_verrijkt_latest.xml
+-rw-r--r--   0        0        0  7917973 2023-06-21 17:43:04.560848 imxinsights-0.0.1.dev13/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml
+-rw-r--r--   0        0        0 15685770 2023-06-21 17:43:04.604848 imxinsights-0.0.1.dev13/sample_data/O_RVTOv2.0_20230602145547.xml
+-rw-r--r--   0        0        0  4762050 2023-06-21 17:43:04.628848 imxinsights-0.0.1.dev13/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml
+-rw-r--r--   0        0        0 15304541 2023-06-21 17:43:04.700849 imxinsights-0.0.1.dev13/sample_data/U_totaal ENL_20230501_compleet_imx500.xml
+-rw-r--r--   0        0        0  1561875 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/sample_data/leeuwarden_verrijkt.xml
+-rw-r--r--   0        0        0      332 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/settings.json
+-rw-r--r--   0        0        0      671 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/setup.cfg
+-rw-r--r--   0        0        0       99 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/test_build.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/tests/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/tests/conftest.py
+-rw-r--r--   0        0        0      616 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/tests/fixtures/files.py
+-rw-r--r--   0        0        0      182 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/tests/fixtures/imx_files.py
+-rw-r--r--   0        0        0      811 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/tests/helpers.py
+-rw-r--r--   0        0        0     7011 2023-06-21 17:43:04.704849 imxinsights-0.0.1.dev13/tests/test_imx.py
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev13/setup.py
+-rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev13/PKG-INFO
```

### Comparing `imxinsights-0.0.1.dev12/.github/workflows/package-build-and-deploy.yml` & `imxinsights-0.0.1.dev13/.github/workflows/package-build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/.github/workflows/python-package-test-build.yml` & `imxinsights-0.0.1.dev13/.github/workflows/python-package-test-build.yml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/.gitignore` & `imxinsights-0.0.1.dev13/.gitignore`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/.idea/inspectionProfiles/Project_Default.xml` & `imxinsights-0.0.1.dev13/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/LICENSE.md` & `imxinsights-0.0.1.dev13/LICENSE.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/Makefile` & `imxinsights-0.0.1.dev13/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 	flake8 ./imxInsights ./tests
 
 typecheck:
 	mypy imxInsights/ tests/
 
 # todo: make sure in production covar is at least 90%
 test:
-	pytest --cov=imxInsights/ --cov-report=term-missing --cov-fail-under=70
+	pytest --cov=imxInsights/ --cov-report=term-missing --cov-fail-under=80
 
 bumpversion-major:
 	bumpversion major
 
 bumpversion-minor:
 	bumpversion minor
```

### Comparing `imxinsights-0.0.1.dev12/README.md` & `imxinsights-0.0.1.dev13/README.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/docs/assets/img/ProRail_logo.svg` & `imxinsights-0.0.1.dev13/docs/assets/img/ProRail_logo.svg`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/docs/examples/advanced/main.py` & `imxinsights-0.0.1.dev13/docs/examples/advanced/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/docs/examples/diff/main.py` & `imxinsights-0.0.1.dev13/docs/examples/diff/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/docs/examples/imx-example.md` & `imxinsights-0.0.1.dev13/docs/examples/imx-example.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/docs/examples/imx/main.py` & `imxinsights-0.0.1.dev13/docs/examples/imx/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/docs/imxInsights/core/imx.md` & `imxinsights-0.0.1.dev13/docs/imxInsights/core/imx.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/docs/imxInsights/core/imxObject.md` & `imxinsights-0.0.1.dev13/docs/imxInsights/core/imxObject.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/docs/notebooks/basic_use.ipynb` & `imxinsights-0.0.1.dev13/docs/notebooks/basic_use.ipynb`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/__init__.py` & `imxinsights-0.0.1.dev13/imxInsights/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1-dev12"
+__version__ = "0.0.1-dev13"
 
 
 from .diff.areaStatusEnum import AreaStatusEnum
 from .diff.change import Change, ChangeList
 from .diff.compair import ImxObjectCompare, ImxPropertyCompare
 from .diff.diffStatusEnum import DiffStatusEnum
 from .diff.imxDiff import ImxDiff
```

### Comparing `imxinsights-0.0.1.dev12/imxInsights/custom_puic_config.yaml` & `imxinsights-0.0.1.dev13/imxInsights/custom_puic_config.yaml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/diff/areaStatusEnum.py` & `imxinsights-0.0.1.dev13/imxInsights/diff/areaStatusEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/diff/change.py` & `imxinsights-0.0.1.dev13/imxInsights/diff/change.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/diff/compair.py` & `imxinsights-0.0.1.dev13/imxInsights/diff/compair.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/diff/diffStatusEnum.py` & `imxinsights-0.0.1.dev13/imxInsights/diff/diffStatusEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/diff/imxDiff.py` & `imxinsights-0.0.1.dev13/imxInsights/diff/imxDiff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from collections import OrderedDict
 from typing import Dict, List, Optional
 
 import pandas as pd
+from shapely.geometry.base import BaseGeometry
 
 from imxInsights.diff.compair import ImxObjectCompare
 from imxInsights.repo.imxRepo import SituationRepo
-from imxInsights.utils.shapely_geojson import (
-    GeoJsonFeature,
-    GeoJsonFeatureCollection,
-    dumps,
-)
+from imxInsights.utils.shapely_geojson import GeoJsonFeature, GeoJsonFeatureCollection
 from imxInsights.utils.shapely_helpers import ShapelyTransform
 
 
 class ImxDiff:
     """
     Calculated difference between two imx situations.
 
@@ -188,64 +185,74 @@
             worksheet.autofilter(0, 0, max_row, max_col - 1)
 
             worksheet.autofit()
             worksheet.freeze_panes(1, 0)
 
         writer.close()
 
-    def as_geojson(self, object_type_or_path: str) -> str:
+    def as_geojson(self, object_type_or_path: str) -> GeoJsonFeatureCollection:
         """
         Returns a geojson of the difference.
 
         Args:
             object_type_or_path:
 
         Returns:
             geojson string
 
         """
-        tester = self._filter_by_types_or_path(object_type_or_path)
         features = []
-        for item in tester:
+        for item in self._filter_by_types_or_path(object_type_or_path):
             difference_dict = item.changes.to_dict()
             if item.diff_status.value == "DELETED":
                 features.append(
                     GeoJsonFeature(
-                        geometry_list=[ShapelyTransform.rd_to_wgs(item.a.shapely)],
+                        geometry_list=[ShapelyTransform.rd_to_wgs(item.a.shapely if item.a.shapely is not None else BaseGeometry())],
                         properties=difference_dict | {"Diff_status": item.diff_status.value},
                     )
                 )
             elif item.diff_status.value == "CREATED":
                 features.append(
                     GeoJsonFeature(
-                        geometry_list=[ShapelyTransform.rd_to_wgs(item.b.shapely)],
+                        geometry_list=[ShapelyTransform.rd_to_wgs(item.b.shapely if item.b.shapely is not None else BaseGeometry())],
                         properties=difference_dict | {"Diff_status": item.diff_status.value},
                     )
                 )
 
             else:
                 features.append(
                     GeoJsonFeature(
-                        geometry_list=[ShapelyTransform.rd_to_wgs(item.a.shapely)],
+                        geometry_list=[ShapelyTransform.rd_to_wgs(item.a.shapely if item.a.shapely is not None else BaseGeometry())],
                         properties=difference_dict | {"Diff_status": item.diff_status.value},
                     )
                 )
                 features.append(
                     GeoJsonFeature(
-                        geometry_list=[ShapelyTransform.rd_to_wgs(item.b.shapely)],
+                        geometry_list=[ShapelyTransform.rd_to_wgs(item.b.shapely if item.b.shapely is not None else BaseGeometry())],
                         properties=difference_dict | {"Diff_status": item.diff_status.value},
                     )
                 )
-        feature_collection = GeoJsonFeatureCollection(geojson_features=features)
-        geojson_str = dumps(feature_collection)
+        return GeoJsonFeatureCollection(geojson_features=features)
 
-        return geojson_str
+    def _get_all_paths(self):
+        return list(set([item.path for item in self._diff]))
 
-    def generate_geojson_dict(self) -> Dict[str, str]:
+    def _get_all_types(self):
+        return list(set([item.tag for item in self._diff]))
+
+    def generate_geojson_dict(self, key_based_on_type: bool = False) -> Dict[str, GeoJsonFeatureCollection]:
         """
         Generates all geojson of the difference.
 
         Todo:
             implement
 
         """
-        raise NotImplementedError
+        out_dict = {}
+        if key_based_on_type:
+            for imx_type in self._get_all_types():
+                out_dict[imx_type] = self.as_geojson(imx_type)
+
+        for imx_path in self._get_all_paths():
+            out_dict[imx_path] = self.as_geojson(imx_path)
+
+        return out_dict
```

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/area/area.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/area/area.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/area/areaClassifiedTypeEnum.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/area/areaClassifiedTypeEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/area/areaClassifier.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/area/areaClassifier.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/area/imxProjectArea.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/area/imxProjectArea.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/imx.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/imx.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/models/ImxRailConnectionInfo.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/models/ImxRailConnectionInfo.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxEnums.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/models/imxEnums.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxGeometry.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/models/imxGeometry.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxMetadata.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/models/imxMetadata.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxPuic.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/models/imxPuic.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxRelation.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/models/imxRelation.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxSituations.py` & `imxinsights-0.0.1.dev13/imxInsights/domain/models/imxSituations.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/repo/imxRepo.py` & `imxinsights-0.0.1.dev13/imxInsights/repo/imxRepo.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/repo/tree/imxTopoTreeObject.py` & `imxinsights-0.0.1.dev13/imxInsights/repo/tree/imxTopoTreeObject.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/repo/tree/imxTreeObject.py` & `imxinsights-0.0.1.dev13/imxInsights/repo/tree/imxTreeObject.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/repo/tree/objectTree.py` & `imxinsights-0.0.1.dev13/imxInsights/repo/tree/objectTree.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/utils/helpers.py` & `imxinsights-0.0.1.dev13/imxInsights/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/utils/log.py` & `imxinsights-0.0.1.dev13/imxInsights/utils/log.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/utils/shapely_geojson.py` & `imxinsights-0.0.1.dev13/imxInsights/utils/shapely_geojson.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/utils/shapely_helpers.py` & `imxinsights-0.0.1.dev13/imxInsights/utils/shapely_helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/imxInsights/utils/xml_helpers.py` & `imxinsights-0.0.1.dev13/imxInsights/utils/xml_helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/mkdocs.yml` & `imxinsights-0.0.1.dev13/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/pyproject.toml` & `imxinsights-0.0.1.dev13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/sample_data/Groningen_verrijkt.xml` & `imxinsights-0.0.1.dev13/sample_data/Groningen_verrijkt.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/sample_data/Hanzelijn_verrijkt_latest.xml` & `imxinsights-0.0.1.dev13/sample_data/Hanzelijn_verrijkt_latest.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml` & `imxinsights-0.0.1.dev13/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/sample_data/O_RVTOv2.0_20230602145547.xml` & `imxinsights-0.0.1.dev13/sample_data/O_RVTOv2.0_20230602145547.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml` & `imxinsights-0.0.1.dev13/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/sample_data/U_totaal ENL_20230501_compleet_imx500.xml` & `imxinsights-0.0.1.dev13/sample_data/U_totaal ENL_20230501_compleet_imx500.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/sample_data/leeuwarden_verrijkt.xml` & `imxinsights-0.0.1.dev13/sample_data/leeuwarden_verrijkt.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/setup.cfg` & `imxinsights-0.0.1.dev13/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [bumpversion]
 commit = True
 tag = True
-current_version = 0.0.1-dev12
+current_version = 0.0.1-dev13
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>.*)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
 
 [bumpversion:part:release]
 optional_value = gamma
```

### Comparing `imxinsights-0.0.1.dev12/tests/fixtures/files.py` & `imxinsights-0.0.1.dev13/tests/fixtures/files.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/tests/helpers.py` & `imxinsights-0.0.1.dev13/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev12/tests/test_imx.py` & `imxinsights-0.0.1.dev13/tests/test_imx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 from pathlib import Path
 
+import pandas as pd
 import pytest
 
 from imxInsights import GeoJsonFeatureCollection, ImxSituationsEnum
-
-# from imxInsights.diff.imxDiff import ImxDiff
+from imxInsights.diff.imxDiff import ImxDiff
 from imxInsights.domain.imx import Imx
 
 
 @pytest.mark.slow
 def test_imx_parse_project_v500(get_imx_project_test_file_path, tmp_path: str):
     imx = Imx(get_imx_project_test_file_path)
+    assert imx.imx_version == "5.0.0", "imx version should be 5.0.0"
 
     imx.generate_population_excel("tester.xlsx", ImxSituationsEnum.NewSituation)
     file_path = Path("tester.xlsx")
     assert file_path.exists(), "file should exist"
     file_path.unlink()
 
     signals_geojson = imx.project.initial_situation.get_geojson(object_type_or_path="Signal")
     assert isinstance(signals_geojson, GeoJsonFeatureCollection), "should return feature collection"
 
-    geojson = imx.project.initial_situation.get_geojson_dict()
-    assert isinstance(geojson, dict), "should return dict"
+    geojson_dict = imx.project.initial_situation.get_geojson_dict()
+    assert isinstance(geojson_dict, dict), "should return dict"
 
-    assert imx.imx_version == "5.0.0", "imx version should be 5.0.0"
+    diff = ImxDiff(imx.project.initial_situation, imx.project.new_situation)
+    signals_geojson_diff = diff.as_geojson(object_type_or_path="Signal")
+    assert isinstance(signals_geojson_diff, GeoJsonFeatureCollection), "should return feature collection"
 
-    # diff = ImxDiff(imx.project.initial_situation, imx.project.new_situation)
-    # dict_of_df_of_all_types = diff.pandas_dataframe_dict()
-    # df_micro_nodes = diff.pandas_dataframe("MicroNode", geometry=False)
-    # df_signals = diff.pandas_dataframe("Signal", geometry=True)
-    # df_rail_con = diff.pandas_dataframe("RailConnection", geometry=True)
-    #
-    # geojson = diff.as_geojson("RailConnection")
-    # diff.generate_excel("./diff.xlsx")
+    geojson_dict_diff = diff.generate_geojson_dict()
+    assert isinstance(geojson_dict_diff, dict), "should return dict"
+
+    dict_of_df_of_all_types = diff.pandas_dataframe_dict()
+    assert isinstance(dict_of_df_of_all_types, dict), "should return dict"
+
+    df_micro_nodes = diff.pandas_dataframe("MicroNode", geometry=False)
+    assert isinstance(df_micro_nodes, pd.DataFrame), "should pd.DataFrame"
+
+    df_signals = diff.pandas_dataframe("Signal", geometry=True)
+    assert isinstance(df_signals, pd.DataFrame), "should pd.DataFrame"
+
+    df_rail_con = diff.pandas_dataframe("RailConnection", geometry=True)
+    assert isinstance(df_rail_con, pd.DataFrame), "should pd.DataFrame"
 
     # signaling_routes = imx.project.initial_situation.get_by_paths("SignalingRoute")
     #
     # rail_cons_missing = []
     # route_missing_rail_cons = []
     # possible_bug = []
     # for signaling_route in signaling_routes:
```

### Comparing `imxinsights-0.0.1.dev12/setup.py` & `imxinsights-0.0.1.dev13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
          'mkdocs-material',
          'mkdocs-mermaid2-plugin',
          'mkdocstrings[crystal, python]>=0.18',
          'pymdown-extensions'],
  'jupyter': ['jupyterlab', 'pygwalker']}
 
 setup(name='imxInsights',
-      version='0.0.1.dev12',
+      version='0.0.1.dev13',
       description='python imx insights module to get information from imx files',
       author=None,
       author_email='Hzd <Hazedd@users.noreply.github.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `imxinsights-0.0.1.dev12/PKG-INFO` & `imxinsights-0.0.1.dev13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imxInsights
-Version: 0.0.1.dev12
+Version: 0.0.1.dev13
 Summary: python imx insights module to get information from imx files
 Author-email: Hzd <Hazedd@users.noreply.github.com>
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3.10
```

