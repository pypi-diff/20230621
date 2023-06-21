# Comparing `tmp/imxinsights-0.0.1.dev11.tar.gz` & `tmp/imxinsights-0.0.1.dev12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imxinsights-0.0.1.dev11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "imxinsights-0.0.1.dev12.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `imxinsights-0.0.1.dev11.tar` & `imxinsights-0.0.1.dev12.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1708 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.github/workflows/package-build-and-deploy.yml
--rw-r--r--   0        0        0     1386 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.github/workflows/python-package-test-build.yml
--rw-r--r--   0        0        0     2700 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.gitignore
--rw-r--r--   0        0        0       47 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/.gitignore
--rw-r--r--   0        0        0      491 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/imxInsightsMonoRepo.iml
--rw-r--r--   0        0        0      817 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      208 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/misc.xml
--rw-r--r--   0        0        0      290 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/modules.xml
--rw-r--r--   0        0        0      180 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/.idea/vcs.xml
--rw-r--r--   0        0        0     1075 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/LICENSE.md
--rw-r--r--   0        0        0     1174 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/Makefile
--rw-r--r--   0        0        0     6378 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/README.md
--rw-r--r--   0        0        0      470 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs-overrides/main.html
--rw-r--r--   0        0        0       71 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/about.md
--rw-r--r--   0        0        0    12851 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/assets/img/ProRail_logo.svg
--rw-r--r--   0        0        0       59 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/contribute.md
--rw-r--r--   0        0        0     1749 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/advanced/main.py
--rw-r--r--   0        0        0       11 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/advanced/requirements.txt
--rw-r--r--   0        0        0      549 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/diff/main.py
--rw-r--r--   0        0        0       11 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/diff/requirements.txt
--rw-r--r--   0        0        0      702 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/imx-example.md
--rw-r--r--   0        0        0     1299 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/imx/main.py
--rw-r--r--   0        0        0       11 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/examples/imx/requirements.txt
--rw-r--r--   0        0        0      439 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/area.md
--rw-r--r--   0        0        0     1005 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/imx.md
--rw-r--r--   0        0        0     1328 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/imxObject.md
--rw-r--r--   0        0        0      441 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/imxPuic.md
--rw-r--r--   0        0        0      282 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/core/imxSituationRepo.md
--rw-r--r--   0        0        0      273 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/diff/change.md
--rw-r--r--   0        0        0      291 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/diff/compare.md
--rw-r--r--   0        0        0      421 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/diff/diff.md
--rw-r--r--   0        0        0      142 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/utils/general.md
--rw-r--r--   0        0        0      149 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/utils/shapely.md
--rw-r--r--   0        0        0      151 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/utils/shapelyGeojson.md
--rw-r--r--   0        0        0      146 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/imxInsights/utils/xml.md
--rw-r--r--   0        0        0       18 2023-06-21 10:18:11.613553 imxinsights-0.0.1.dev11/docs/index.md
--rw-r--r--   0        0        0  4713938 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/docs/notebooks/basic_use.ipynb
--rw-r--r--   0        0        0     2281 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/__init__.py
--rw-r--r--   0        0        0      840 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/custom_puic_config.yaml
--rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/__init__.py
--rw-r--r--   0        0        0      900 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/areaStatusEnum.py
--rw-r--r--   0        0        0     4313 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/change.py
--rw-r--r--   0        0        0    10668 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/compair.py
--rw-r--r--   0        0        0      889 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/diffStatusEnum.py
--rw-r--r--   0        0        0     9026 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/diff/imxDiff.py
--rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/__init__.py
--rw-r--r--   0        0        0      657 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/area.py
--rw-r--r--   0        0        0      638 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/areaClassifiedTypeEnum.py
--rw-r--r--   0        0        0     5280 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/areaClassifier.py
--rw-r--r--   0        0        0     3100 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/area/imxProjectArea.py
--rw-r--r--   0        0        0     5980 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/imx.py
--rw-r--r--   0        0        0     3554 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/ImxRailConnectionInfo.py
--rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/__init__.py
--rw-r--r--   0        0        0      753 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxEnums.py
--rw-r--r--   0        0        0     1002 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxGeometry.py
--rw-r--r--   0        0        0     9417 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxMetadata.py
--rw-r--r--   0        0        0     5657 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxPuic.py
--rw-r--r--   0        0        0      885 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxRelation.py
--rw-r--r--   0        0        0     3990 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/domain/models/imxSituations.py
--rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/__init__.py
--rw-r--r--   0        0        0    19150 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/imxRepo.py
--rw-r--r--   0        0        0        0 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/tree/__init__.py
--rw-r--r--   0        0        0     1199 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/tree/imxTopoTreeObject.py
--rw-r--r--   0        0        0     7924 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/tree/imxTreeObject.py
--rw-r--r--   0        0        0     4132 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/repo/tree/objectTree.py
--rw-r--r--   0        0        0       56 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/__init__.py
--rw-r--r--   0        0        0     3653 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/helpers.py
--rw-r--r--   0        0        0     1308 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/log.py
--rw-r--r--   0        0        0     5778 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/shapely_geojson.py
--rw-r--r--   0        0        0     3808 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/shapely_helpers.py
--rw-r--r--   0        0        0     3620 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/imxInsights/utils/xml_helpers.py
--rw-r--r--   0        0        0     2470 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/mkdocs.yml
--rw-r--r--   0        0        0     1798 2023-06-21 10:18:11.633553 imxinsights-0.0.1.dev11/pyproject.toml
--rw-r--r--   0        0        0  7366031 2023-06-21 10:18:11.657553 imxinsights-0.0.1.dev11/sample_data/Groningen_verrijkt.xml
--rw-r--r--   0        0        0 10387299 2023-06-21 10:18:11.685553 imxinsights-0.0.1.dev11/sample_data/Hanzelijn_verrijkt_latest.xml
--rw-r--r--   0        0        0  7917973 2023-06-21 10:18:11.737553 imxinsights-0.0.1.dev11/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml
--rw-r--r--   0        0        0 15685770 2023-06-21 10:18:11.785554 imxinsights-0.0.1.dev11/sample_data/O_RVTOv2.0_20230602145547.xml
--rw-r--r--   0        0        0  4762050 2023-06-21 10:18:11.809553 imxinsights-0.0.1.dev11/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml
--rw-r--r--   0        0        0 15304541 2023-06-21 10:18:11.889554 imxinsights-0.0.1.dev11/sample_data/U_totaal ENL_20230501_compleet_imx500.xml
--rw-r--r--   0        0        0  1561875 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/sample_data/leeuwarden_verrijkt.xml
--rw-r--r--   0        0        0      332 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/settings.json
--rw-r--r--   0        0        0      671 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/setup.cfg
--rw-r--r--   0        0        0       99 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/test_build.py
--rw-r--r--   0        0        0        0 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/__init__.py
--rw-r--r--   0        0        0      133 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/conftest.py
--rw-r--r--   0        0        0      616 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/fixtures/files.py
--rw-r--r--   0        0        0      182 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/fixtures/imx_files.py
--rw-r--r--   0        0        0      811 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/helpers.py
--rw-r--r--   0        0        0     6497 2023-06-21 10:18:11.893554 imxinsights-0.0.1.dev11/tests/test_imx.py
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev11/setup.py
--rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev11/PKG-INFO
+-rw-r--r--   0        0        0     1708 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.github/workflows/package-build-and-deploy.yml
+-rw-r--r--   0        0        0     1417 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.github/workflows/python-package-test-build.yml
+-rw-r--r--   0        0        0     2700 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.gitignore
+-rw-r--r--   0        0        0       47 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/.gitignore
+-rw-r--r--   0        0        0      491 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/imxInsightsMonoRepo.iml
+-rw-r--r--   0        0        0      817 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      208 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/misc.xml
+-rw-r--r--   0        0        0      290 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/.idea/vcs.xml
+-rw-r--r--   0        0        0     1075 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/LICENSE.md
+-rw-r--r--   0        0        0     1174 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/Makefile
+-rw-r--r--   0        0        0     6378 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/README.md
+-rw-r--r--   0        0        0      470 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs-overrides/main.html
+-rw-r--r--   0        0        0       71 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/about.md
+-rw-r--r--   0        0        0    12851 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/assets/img/ProRail_logo.svg
+-rw-r--r--   0        0        0       59 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/contribute.md
+-rw-r--r--   0        0        0     1749 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/advanced/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/advanced/requirements.txt
+-rw-r--r--   0        0        0      549 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/diff/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/diff/requirements.txt
+-rw-r--r--   0        0        0      702 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/imx-example.md
+-rw-r--r--   0        0        0     1299 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/imx/main.py
+-rw-r--r--   0        0        0       11 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/examples/imx/requirements.txt
+-rw-r--r--   0        0        0      439 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/area.md
+-rw-r--r--   0        0        0     1005 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/imx.md
+-rw-r--r--   0        0        0     1328 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/imxObject.md
+-rw-r--r--   0        0        0      441 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/imxPuic.md
+-rw-r--r--   0        0        0      282 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/core/imxSituationRepo.md
+-rw-r--r--   0        0        0      273 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/diff/change.md
+-rw-r--r--   0        0        0      291 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/diff/compare.md
+-rw-r--r--   0        0        0      421 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/diff/diff.md
+-rw-r--r--   0        0        0      142 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/utils/general.md
+-rw-r--r--   0        0        0      149 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/utils/shapely.md
+-rw-r--r--   0        0        0      151 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/utils/shapelyGeojson.md
+-rw-r--r--   0        0        0      146 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/imxInsights/utils/xml.md
+-rw-r--r--   0        0        0       18 2023-06-21 15:08:22.840445 imxinsights-0.0.1.dev12/docs/index.md
+-rw-r--r--   0        0        0  4713938 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/docs/notebooks/basic_use.ipynb
+-rw-r--r--   0        0        0     2281 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/imxInsights/__init__.py
+-rw-r--r--   0        0        0      840 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/imxInsights/custom_puic_config.yaml
+-rw-r--r--   0        0        0        0 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/imxInsights/diff/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-21 15:08:22.856445 imxinsights-0.0.1.dev12/imxInsights/diff/areaStatusEnum.py
+-rw-r--r--   0        0        0     4313 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/diff/change.py
+-rw-r--r--   0        0        0    10668 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/diff/compair.py
+-rw-r--r--   0        0        0      889 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/diff/diffStatusEnum.py
+-rw-r--r--   0        0        0     9026 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/diff/imxDiff.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/__init__.py
+-rw-r--r--   0        0        0      657 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/area.py
+-rw-r--r--   0        0        0      638 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/areaClassifiedTypeEnum.py
+-rw-r--r--   0        0        0     5280 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/areaClassifier.py
+-rw-r--r--   0        0        0     3100 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/area/imxProjectArea.py
+-rw-r--r--   0        0        0     6905 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/imx.py
+-rw-r--r--   0        0        0     3554 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/ImxRailConnectionInfo.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxEnums.py
+-rw-r--r--   0        0        0     1002 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxGeometry.py
+-rw-r--r--   0        0        0     9417 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxMetadata.py
+-rw-r--r--   0        0        0     5657 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxPuic.py
+-rw-r--r--   0        0        0      885 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxRelation.py
+-rw-r--r--   0        0        0     3990 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/domain/models/imxSituations.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/__init__.py
+-rw-r--r--   0        0        0    19150 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/imxRepo.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/tree/__init__.py
+-rw-r--r--   0        0        0     1199 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/tree/imxTopoTreeObject.py
+-rw-r--r--   0        0        0     7924 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/tree/imxTreeObject.py
+-rw-r--r--   0        0        0     4132 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/repo/tree/objectTree.py
+-rw-r--r--   0        0        0       56 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/__init__.py
+-rw-r--r--   0        0        0     3653 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/helpers.py
+-rw-r--r--   0        0        0     1308 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/log.py
+-rw-r--r--   0        0        0     5778 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/shapely_geojson.py
+-rw-r--r--   0        0        0     3808 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/shapely_helpers.py
+-rw-r--r--   0        0        0     3620 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/imxInsights/utils/xml_helpers.py
+-rw-r--r--   0        0        0     2470 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/mkdocs.yml
+-rw-r--r--   0        0        0     1798 2023-06-21 15:08:22.860445 imxinsights-0.0.1.dev12/pyproject.toml
+-rw-r--r--   0        0        0  7366031 2023-06-21 15:08:22.880446 imxinsights-0.0.1.dev12/sample_data/Groningen_verrijkt.xml
+-rw-r--r--   0        0        0 10387299 2023-06-21 15:08:22.912446 imxinsights-0.0.1.dev12/sample_data/Hanzelijn_verrijkt_latest.xml
+-rw-r--r--   0        0        0  7917973 2023-06-21 15:08:22.960447 imxinsights-0.0.1.dev12/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml
+-rw-r--r--   0        0        0 15685770 2023-06-21 15:08:23.004447 imxinsights-0.0.1.dev12/sample_data/O_RVTOv2.0_20230602145547.xml
+-rw-r--r--   0        0        0  4762050 2023-06-21 15:08:23.028448 imxinsights-0.0.1.dev12/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml
+-rw-r--r--   0        0        0 15304541 2023-06-21 15:08:23.104449 imxinsights-0.0.1.dev12/sample_data/U_totaal ENL_20230501_compleet_imx500.xml
+-rw-r--r--   0        0        0  1561875 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/sample_data/leeuwarden_verrijkt.xml
+-rw-r--r--   0        0        0      332 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/settings.json
+-rw-r--r--   0        0        0      671 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/setup.cfg
+-rw-r--r--   0        0        0       99 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/test_build.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/conftest.py
+-rw-r--r--   0        0        0      616 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/fixtures/files.py
+-rw-r--r--   0        0        0      182 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/fixtures/imx_files.py
+-rw-r--r--   0        0        0      811 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/helpers.py
+-rw-r--r--   0        0        0     6493 2023-06-21 15:08:23.108449 imxinsights-0.0.1.dev12/tests/test_imx.py
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev12/setup.py
+-rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 imxinsights-0.0.1.dev12/PKG-INFO
```

### Comparing `imxinsights-0.0.1.dev11/.github/workflows/package-build-and-deploy.yml` & `imxinsights-0.0.1.dev12/.github/workflows/package-build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/.github/workflows/python-package-test-build.yml` & `imxinsights-0.0.1.dev12/.github/workflows/python-package-test-build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -47,8 +47,9 @@
         flit build --setup-py
         flit install --deps none --python $(which python)
         python test_build.py
 
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
+        python-version: '3.10'
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `imxinsights-0.0.1.dev11/.gitignore` & `imxinsights-0.0.1.dev12/.gitignore`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/.idea/inspectionProfiles/Project_Default.xml` & `imxinsights-0.0.1.dev12/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/LICENSE.md` & `imxinsights-0.0.1.dev12/LICENSE.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/Makefile` & `imxinsights-0.0.1.dev12/Makefile`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/README.md` & `imxinsights-0.0.1.dev12/README.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/docs/assets/img/ProRail_logo.svg` & `imxinsights-0.0.1.dev12/docs/assets/img/ProRail_logo.svg`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/docs/examples/advanced/main.py` & `imxinsights-0.0.1.dev12/docs/examples/advanced/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/docs/examples/diff/main.py` & `imxinsights-0.0.1.dev12/docs/examples/diff/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/docs/examples/imx-example.md` & `imxinsights-0.0.1.dev12/docs/examples/imx-example.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/docs/examples/imx/main.py` & `imxinsights-0.0.1.dev12/docs/examples/imx/main.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/docs/imxInsights/core/imx.md` & `imxinsights-0.0.1.dev12/docs/imxInsights/core/imx.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/docs/imxInsights/core/imxObject.md` & `imxinsights-0.0.1.dev12/docs/imxInsights/core/imxObject.md`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/docs/notebooks/basic_use.ipynb` & `imxinsights-0.0.1.dev12/docs/notebooks/basic_use.ipynb`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/__init__.py` & `imxinsights-0.0.1.dev12/imxInsights/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1-dev11"
+__version__ = "0.0.1-dev12"
 
 
 from .diff.areaStatusEnum import AreaStatusEnum
 from .diff.change import Change, ChangeList
 from .diff.compair import ImxObjectCompare, ImxPropertyCompare
 from .diff.diffStatusEnum import DiffStatusEnum
 from .diff.imxDiff import ImxDiff
```

### Comparing `imxinsights-0.0.1.dev11/imxInsights/custom_puic_config.yaml` & `imxinsights-0.0.1.dev12/imxInsights/custom_puic_config.yaml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/diff/areaStatusEnum.py` & `imxinsights-0.0.1.dev12/imxInsights/diff/areaStatusEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/diff/change.py` & `imxinsights-0.0.1.dev12/imxInsights/diff/change.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/diff/compair.py` & `imxinsights-0.0.1.dev12/imxInsights/diff/compair.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/diff/diffStatusEnum.py` & `imxinsights-0.0.1.dev12/imxInsights/diff/diffStatusEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/diff/imxDiff.py` & `imxinsights-0.0.1.dev12/imxInsights/diff/imxDiff.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/area/area.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/area/area.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/area/areaClassifiedTypeEnum.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/area/areaClassifiedTypeEnum.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/area/areaClassifier.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/area/areaClassifier.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/area/imxProjectArea.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/area/imxProjectArea.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/imx.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/imx.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,23 +70,24 @@
 
         else:
             if self.situation is not None:
                 return self.situation
             return None
 
     @staticmethod
-    def _reshape_df_worksheet(df, worksheet):
+    def _reshape_df_worksheet(df, worksheet, filter=True):
         # Get the dimensions of the dataframe.
         (max_row, max_col) = df.shape
 
         # Make the columns wider for clarity.
         worksheet.set_column(0, max_col - 1, 12)
 
-        # Set the autofilter.
-        worksheet.autofilter(0, 0, max_row, max_col - 1)
+        if filter:
+            # Set the autofilter.
+            worksheet.autofilter(0, 0, max_row, max_col)
 
         worksheet.autofit()
         worksheet.freeze_panes(1, 0)
 
     def generate_population_excel(self, file_path: str, situation: ImxSituationsEnum):
         repo = self.get_situation_repository(situation)
 
@@ -99,16 +100,17 @@
 
         worksheet_info.write(0, 0, "file")
         worksheet_info.write(0, 1, self.file_path.name)
         worksheet_info.write(1, 0, "imx version")
         worksheet_info.write(1, 1, self.imx_version)
         worksheet_info.write(2, 0, "sha256")
         worksheet_info.write(2, 1, sha256sum(self.file_path.resolve()))
+        worksheet_info.write(3, 0, "situation")
+        worksheet_info.write(3, 1, situation.value)
 
-        # todo: create overview count on area
         overview_records = []
         overview_keys_to_keep = [
             "puic",
             "path",
             "area",
             "name",
             "parent",
@@ -119,44 +121,67 @@
             "Metadata.@isInService",
             "Location.GeographicLocation.@dataAcquisitionMethod",
             "Location.GeographicLocation.@accuracy",
         ]
 
         df_dict = repo.get_pandas_df_dict()
 
+        pivot_index = [
+            "path",
+            "Metadata.@lifeCycleStatus",
+            "Location.GeographicLocation.@accuracy",
+            "Location.GeographicLocation.@dataAcquisitionMethod",
+        ]
+
         for key, df in df_dict.items():
             records_ = df.to_dict(orient="records")
+
             for record_ in records_:
                 records_to_add = {key: value for key, value in record_.items() if key in overview_keys_to_keep} | {"counter": 1}
+                if records_to_add["parent"] == "":
+                    records_to_add["_parent"] = records_to_add["puic"]
+                else:
+                    records_to_add["_parent"] = records_to_add["parent"]
+
+                for item in pivot_index:
+                    if item not in records_to_add.keys():
+                        records_to_add[item] = ""
+
                 overview_records.append(records_to_add)
 
         df = pd.DataFrame.from_records(overview_records)
 
         # create pivot
         table = pd.pivot_table(
             df,
             values="counter",
-            index=[
-                "path",
-                "Metadata.@lifeCycleStatus",
-                "Location.GeographicLocation.@accuracy",
-                "Location.GeographicLocation.@dataAcquisitionMethod",
-            ],
+            index=pivot_index,
             columns=["area"],
             aggfunc="count",
-            fill_value=0,
+            fill_value=" ",
         )
         table.to_excel(writer, sheet_name="population_pivot", index=True)
         worksheet = writer.sheets["population_pivot"]
-        self._reshape_df_worksheet(table, worksheet)
+        self._reshape_df_worksheet(table, worksheet, filter=False)
+
+        temp_df = df["path"].str.split(".", expand=True)
+        df["main_type"] = temp_df[0]
         del df["counter"]
 
+        df_grouped = df.groupby(["main_type", "_parent", "path"], group_keys=True).apply(lambda group: group)
+        df_grouped = df_grouped.assign(row_number=range(len(df)))
+        df = df_grouped.set_index("row_number")
+
+        first_column = df.pop("main_type")
+        df.insert(2, "main_type", first_column)
+        del df["_parent"]
+
         df.to_excel(writer, sheet_name="all_objects", startrow=0, startcol=0, index=1)
         worksheet = writer.sheets["all_objects"]
-        self._reshape_df_worksheet(table, worksheet)
+        self._reshape_df_worksheet(df, worksheet)
 
         for key, df in sorted(df_dict.items()):
             records_ = df.to_dict(orient="records")
             for record_ in records_:
                 records_to_add = {key: value for key, value in record_.items() if key in overview_keys_to_keep}
                 overview_records.append(records_to_add)
```

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/models/ImxRailConnectionInfo.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/models/ImxRailConnectionInfo.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxEnums.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxEnums.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxGeometry.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxGeometry.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxMetadata.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxMetadata.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxPuic.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxPuic.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxRelation.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxRelation.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/domain/models/imxSituations.py` & `imxinsights-0.0.1.dev12/imxInsights/domain/models/imxSituations.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/repo/imxRepo.py` & `imxinsights-0.0.1.dev12/imxInsights/repo/imxRepo.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/repo/tree/imxTopoTreeObject.py` & `imxinsights-0.0.1.dev12/imxInsights/repo/tree/imxTopoTreeObject.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/repo/tree/imxTreeObject.py` & `imxinsights-0.0.1.dev12/imxInsights/repo/tree/imxTreeObject.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/repo/tree/objectTree.py` & `imxinsights-0.0.1.dev12/imxInsights/repo/tree/objectTree.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/utils/helpers.py` & `imxinsights-0.0.1.dev12/imxInsights/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/utils/log.py` & `imxinsights-0.0.1.dev12/imxInsights/utils/log.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/utils/shapely_geojson.py` & `imxinsights-0.0.1.dev12/imxInsights/utils/shapely_geojson.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/utils/shapely_helpers.py` & `imxinsights-0.0.1.dev12/imxInsights/utils/shapely_helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/imxInsights/utils/xml_helpers.py` & `imxinsights-0.0.1.dev12/imxInsights/utils/xml_helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/mkdocs.yml` & `imxinsights-0.0.1.dev12/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/pyproject.toml` & `imxinsights-0.0.1.dev12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/sample_data/Groningen_verrijkt.xml` & `imxinsights-0.0.1.dev12/sample_data/Groningen_verrijkt.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/sample_data/Hanzelijn_verrijkt_latest.xml` & `imxinsights-0.0.1.dev12/sample_data/Hanzelijn_verrijkt_latest.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml` & `imxinsights-0.0.1.dev12/sample_data/IMX_E-R50008_EKB_Perceel_2_V1.3_5_0_0_test_Niki.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/sample_data/O_RVTOv2.0_20230602145547.xml` & `imxinsights-0.0.1.dev12/sample_data/O_RVTOv2.0_20230602145547.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml` & `imxinsights-0.0.1.dev12/sample_data/U_O_D-003122_ERTMS_Noordelijke_lijnen_TVP01_Leeu_01_20230417_compleet_concept_imx500.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/sample_data/U_totaal ENL_20230501_compleet_imx500.xml` & `imxinsights-0.0.1.dev12/sample_data/U_totaal ENL_20230501_compleet_imx500.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/sample_data/leeuwarden_verrijkt.xml` & `imxinsights-0.0.1.dev12/sample_data/leeuwarden_verrijkt.xml`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/setup.cfg` & `imxinsights-0.0.1.dev12/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [bumpversion]
 commit = True
 tag = True
-current_version = 0.0.1-dev11
+current_version = 0.0.1-dev12
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>.*)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
 
 [bumpversion:part:release]
 optional_value = gamma
```

### Comparing `imxinsights-0.0.1.dev11/tests/fixtures/files.py` & `imxinsights-0.0.1.dev12/tests/fixtures/files.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/tests/helpers.py` & `imxinsights-0.0.1.dev12/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `imxinsights-0.0.1.dev11/tests/test_imx.py` & `imxinsights-0.0.1.dev12/tests/test_imx.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from imxInsights.domain.imx import Imx
 
 
 @pytest.mark.slow
 def test_imx_parse_project_v500(get_imx_project_test_file_path, tmp_path: str):
     imx = Imx(get_imx_project_test_file_path)
 
-    imx.generate_population_excel("tester.xlsx", ImxSituationsEnum.InitialSituation)
+    imx.generate_population_excel("tester.xlsx", ImxSituationsEnum.NewSituation)
     file_path = Path("tester.xlsx")
     assert file_path.exists(), "file should exist"
     file_path.unlink()
 
     signals_geojson = imx.project.initial_situation.get_geojson(object_type_or_path="Signal")
     assert isinstance(signals_geojson, GeoJsonFeatureCollection), "should return feature collection"
```

### Comparing `imxinsights-0.0.1.dev11/setup.py` & `imxinsights-0.0.1.dev12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
          'mkdocs-material',
          'mkdocs-mermaid2-plugin',
          'mkdocstrings[crystal, python]>=0.18',
          'pymdown-extensions'],
  'jupyter': ['jupyterlab', 'pygwalker']}
 
 setup(name='imxInsights',
-      version='0.0.1.dev11',
+      version='0.0.1.dev12',
       description='python imx insights module to get information from imx files',
       author=None,
       author_email='Hzd <Hazedd@users.noreply.github.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `imxinsights-0.0.1.dev11/PKG-INFO` & `imxinsights-0.0.1.dev12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imxInsights
-Version: 0.0.1.dev11
+Version: 0.0.1.dev12
 Summary: python imx insights module to get information from imx files
 Author-email: Hzd <Hazedd@users.noreply.github.com>
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3.10
```

