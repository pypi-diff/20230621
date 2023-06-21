# Comparing `tmp/osm-fieldwork-0.3.1rc1.tar.gz` & `tmp/osm-fieldwork-0.3.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-fieldwork-0.3.1rc1.tar", last modified: Thu May 18 15:06:20 2023, max compression
+gzip compressed data, was "osm-fieldwork-0.3.1rc2.tar", last modified: Thu Jun  1 17:30:39 2023, max compression
```

## Comparing `osm-fieldwork-0.3.1rc1.tar` & `osm-fieldwork-0.3.1rc2.tar`

### file list

```diff
@@ -1,83 +1,85 @@
--rw-r--r--   0        0        0    34625 2023-05-18 15:06:13.381338 osm-fieldwork-0.3.1rc1/LICENSE.md
--rw-r--r--   0        0        0     8656 2023-05-18 15:06:13.381338 osm-fieldwork-0.3.1rc1/README.md
--rwxr-xr-x   0        0        0    13091 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/CSVDump.py
--rwxr-xr-x   0        0        0     5099 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/ODKDump.py
--rwxr-xr-x   0        0        0     4400 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/ODKForm.py
--rwxr-xr-x   0        0        0     8761 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/ODKInstance.py
--rwxr-xr-x   0        0        0    26764 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/OdkCentral.py
--rw-r--r--   0        0        0        0 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/__init__.py
--rw-r--r--   0        0        0       25 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/__version__.py
--rwxr-xr-x   0        0        0     9432 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/basemapper.py
--rwxr-xr-x   0        0        0     9631 2023-05-18 15:06:13.385337 osm-fieldwork-0.3.1rc1/osm_fieldwork/convert.py
--rw-r--r--   0        0        0   683456 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
--rw-r--r--   0        0        0      366 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/amenities.yaml
--rw-r--r--   0        0        0      226 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/buildings.yaml
--rw-r--r--   0        0        0      240 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/camping.yaml
--rw-r--r--   0        0        0      678 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/category.yaml
--rw-r--r--   0        0        0      119 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/cemeteries.yaml
--rw-r--r--   0        0        0      412 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/education.yaml
--rw-r--r--   0        0        0      137 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/emergency.yaml
--rw-r--r--   0        0        0      495 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/health.yaml
--rw-r--r--   0        0        0       94 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/landusage.yaml
--rw-r--r--   0        0        0    14028 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/models.yaml
--rw-r--r--   0        0        0      106 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/nature.yaml
--rw-r--r--   0        0        0      104 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/places.yaml
--rw-r--r--   0        0        0      107 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/religious.yaml
--rw-r--r--   0        0        0      245 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/toilets.yaml
--rwxr-xr-x   0        0        0     4745 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/validate.py
--rw-r--r--   0        0        0      348 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/wastedisposal.yaml
--rw-r--r--   0        0        0      170 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/waterpoints.yaml
--rw-r--r--   0        0        0      140 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/waterways.yaml
--rw-r--r--   0        0        0     1609 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/filter.yaml
--rwxr-xr-x   0        0        0     7378 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/filter_data.py
--rwxr-xr-x   0        0        0    13298 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/json2osm.py
--rwxr-xr-x   0        0        0    18443 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/make_data_extract.py
--rwxr-xr-x   0        0        0     5254 2023-05-18 15:06:13.389338 osm-fieldwork-0.3.1rc1/osm_fieldwork/odk2csv.py
--rwxr-xr-x   0        0        0    13642 2023-05-18 15:06:13.393338 osm-fieldwork-0.3.1rc1/osm_fieldwork/odk_client.py
--rwxr-xr-x   0        0        0     8766 2023-05-18 15:06:13.393338 osm-fieldwork-0.3.1rc1/osm_fieldwork/odk_merge.py
--rwxr-xr-x   0        0        0    11519 2023-05-18 15:06:13.393338 osm-fieldwork-0.3.1rc1/osm_fieldwork/osmfile.py
--rwxr-xr-x   0        0        0     8003 2023-05-18 15:06:13.393338 osm-fieldwork-0.3.1rc1/osm_fieldwork/sqlite.py
--rw-r--r--   0        0        0     4487 2023-05-18 15:06:13.393338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xforms.yaml
--rw-r--r--   0        0        0     3800 2023-05-18 15:06:13.393338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/Makefile
--rw-r--r--   0        0        0      830 2023-05-18 15:06:13.393338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/__init__.py
--rw-r--r--   0        0        0  1469440 2023-05-18 15:06:13.397338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/amenities.xls
--rw-r--r--   0        0        0   240128 2023-05-18 15:06:13.397338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/buildings.xls
--rw-r--r--   0        0        0  3986944 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/camping.xls
--rw-r--r--   0        0        0    98816 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/cemeteries.xls
--rw-r--r--   0        0        0   111104 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/education.xls
--rw-r--r--   0        0        0    69120 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/health.xls
--rw-r--r--   0        0        0    22528 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/historical.xls
--rw-r--r--   0        0        0    15872 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/hotspring.xls
--rw-r--r--   0        0        0    59904 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/landusage.xls
--rw-r--r--   0        0        0   129536 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/landuse.xls
--rw-r--r--   0        0        0     1629 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/amenities.csv
--rw-r--r--   0        0        0      466 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/buildings.csv
--rw-r--r--   0        0        0       40 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/municipality.csv
--rw-r--r--   0        0        0      353 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/opening_hours.csv
--rw-r--r--   0        0        0      160 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/operational_status.csv
--rw-r--r--   0        0        0      171 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/provider.csv
--rw-r--r--   0        0        0     1737 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/towns.csv
--rw-r--r--   0        0        0       76 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/waste.csv
--rw-r--r--   0        0        0       41 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/municipality.csv
--rw-r--r--   0        0        0    59392 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/nature.xls
--rw-r--r--   0        0        0   126976 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/places.xls
--rw-r--r--   0        0        0   103424 2023-05-18 15:06:13.409338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/religious.xls
--rw-r--r--   0        0        0  1537536 2023-05-18 15:06:13.413338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/slides.xls
--rw-r--r--   0        0        0   115963 2023-05-18 15:06:13.413338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/solidwaste.xlsx
--rw-r--r--   0        0        0   118272 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/toilets.xls
--rw-r--r--   0        0        0      112 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/towns.csv
--rw-r--r--   0        0        0    40448 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/transportation.xls
--rw-r--r--   0        0        0    15186 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/waste_collection.xlsx
--rw-r--r--   0        0        0   101888 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/wastedisposal.xls
--rw-r--r--   0        0        0   211456 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/waterpoints.xls
--rw-r--r--   0        0        0   269312 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/waterways.xls
--rwxr-xr-x   0        0        0     3726 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/osm_fieldwork/yamlfile.py
--rw-r--r--   0        0        0     1694 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/tests/.flake8
--rw-r--r--   0        0        0      574 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/tests/Test.yaml
--rw-r--r--   0        0        0     2713 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/tests/test.csv
--rwxr-xr-x   0        0        0     2324 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/tests/test_convert.py
--rwxr-xr-x   0        0        0     1889 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/tests/test_csv.py
--rwxr-xr-x   0        0        0     3204 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/tests/test_osm.py
--rwxr-xr-x   0        0        0     1649 2023-05-18 15:06:13.417338 osm-fieldwork-0.3.1rc1/tests/test_yaml.py
--rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 osm-fieldwork-0.3.1rc1/PKG-INFO
+-rw-r--r--   0        0        0    34625 2023-06-01 17:30:33.408398 osm-fieldwork-0.3.1rc2/LICENSE.md
+-rw-r--r--   0        0        0     8656 2023-06-01 17:30:33.408398 osm-fieldwork-0.3.1rc2/README.md
+-rwxr-xr-x   0        0        0    13091 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/CSVDump.py
+-rwxr-xr-x   0        0        0     5099 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKDump.py
+-rwxr-xr-x   0        0        0     4400 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKForm.py
+-rwxr-xr-x   0        0        0     4205 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKInstance.py
+-rwxr-xr-x   0        0        0    27428 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/OdkCentral.py
+-rw-r--r--   0        0        0        0 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/__version__.py
+-rwxr-xr-x   0        0        0     9588 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/basemapper.py
+-rwxr-xr-x   0        0        0     9631 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/convert.py
+-rw-r--r--   0        0        0   683456 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
+-rw-r--r--   0        0        0      366 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/amenities.yaml
+-rw-r--r--   0        0        0      226 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/buildings.yaml
+-rw-r--r--   0        0        0      240 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/camping.yaml
+-rw-r--r--   0        0        0      678 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/category.yaml
+-rw-r--r--   0        0        0      119 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/cemeteries.yaml
+-rw-r--r--   0        0        0      412 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/education.yaml
+-rw-r--r--   0        0        0      137 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/emergency.yaml
+-rw-r--r--   0        0        0      495 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/health.yaml
+-rw-r--r--   0        0        0       94 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/landusage.yaml
+-rw-r--r--   0        0        0    14028 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/models.yaml
+-rw-r--r--   0        0        0      106 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/nature.yaml
+-rw-r--r--   0        0        0      104 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/places.yaml
+-rw-r--r--   0        0        0      107 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/religious.yaml
+-rw-r--r--   0        0        0      245 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/toilets.yaml
+-rwxr-xr-x   0        0        0     4745 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/validate.py
+-rw-r--r--   0        0        0      348 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/wastedisposal.yaml
+-rw-r--r--   0        0        0      170 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/waterpoints.yaml
+-rw-r--r--   0        0        0      140 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/waterways.yaml
+-rw-r--r--   0        0        0     1609 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/filter.yaml
+-rwxr-xr-x   0        0        0     7378 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/filter_data.py
+-rwxr-xr-x   0        0        0    16479 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/json2osm.py
+-rwxr-xr-x   0        0        0    18443 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/make_data_extract.py
+-rwxr-xr-x   0        0        0     5254 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/odk2csv.py
+-rwxr-xr-x   0        0        0     4199 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/odk2geojson.py
+-rwxr-xr-x   0        0        0    13649 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/odk_client.py
+-rwxr-xr-x   0        0        0     8766 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/odk_merge.py
+-rwxr-xr-x   0        0        0     5036 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/osm2favorities.py
+-rwxr-xr-x   0        0        0    11537 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/osmfile.py
+-rwxr-xr-x   0        0        0     8003 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/sqlite.py
+-rw-r--r--   0        0        0     4474 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/xforms.yaml
+-rw-r--r--   0        0        0     3800 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/Makefile
+-rw-r--r--   0        0        0      830 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/__init__.py
+-rw-r--r--   0        0        0  1469440 2023-06-01 17:30:33.420399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/amenities.xls
+-rw-r--r--   0        0        0   240128 2023-06-01 17:30:33.420399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/buildings.xls
+-rw-r--r--   0        0        0  3986944 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/camping.xls
+-rw-r--r--   0        0        0    98816 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/cemeteries.xls
+-rw-r--r--   0        0        0   111104 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/education.xls
+-rw-r--r--   0        0        0    69120 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/health.xls
+-rw-r--r--   0        0        0    22528 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/historical.xls
+-rw-r--r--   0        0        0    15872 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/hotspring.xls
+-rw-r--r--   0        0        0    59904 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/landusage.xls
+-rw-r--r--   0        0        0   129536 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/landuse.xls
+-rw-r--r--   0        0        0     1629 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/amenities.csv
+-rw-r--r--   0        0        0      466 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/buildings.csv
+-rw-r--r--   0        0        0       40 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/municipality.csv
+-rw-r--r--   0        0        0      353 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/opening_hours.csv
+-rw-r--r--   0        0        0      160 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/operational_status.csv
+-rw-r--r--   0        0        0      171 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/provider.csv
+-rw-r--r--   0        0        0     1737 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/towns.csv
+-rw-r--r--   0        0        0       76 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/waste.csv
+-rw-r--r--   0        0        0       41 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/municipality.csv
+-rw-r--r--   0        0        0    59392 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/nature.xls
+-rw-r--r--   0        0        0   126976 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/places.xls
+-rw-r--r--   0        0        0   103424 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/religious.xls
+-rw-r--r--   0        0        0  1537536 2023-06-01 17:30:33.436399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/slides.xls
+-rw-r--r--   0        0        0   115963 2023-06-01 17:30:33.436399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/solidwaste.xlsx
+-rw-r--r--   0        0        0   118272 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/toilets.xls
+-rw-r--r--   0        0        0      112 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/towns.csv
+-rw-r--r--   0        0        0    40448 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/transportation.xls
+-rw-r--r--   0        0        0    15186 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waste_collection.xlsx
+-rw-r--r--   0        0        0   101888 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/wastedisposal.xls
+-rw-r--r--   0        0        0   211456 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waterpoints.xls
+-rw-r--r--   0        0        0   269312 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waterways.xls
+-rwxr-xr-x   0        0        0     3726 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/yamlfile.py
+-rw-r--r--   0        0        0     1694 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/.flake8
+-rw-r--r--   0        0        0      574 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/Test.yaml
+-rw-r--r--   0        0        0     2713 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test.csv
+-rwxr-xr-x   0        0        0     2324 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test_convert.py
+-rwxr-xr-x   0        0        0     1889 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test_csv.py
+-rwxr-xr-x   0        0        0     3204 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test_osm.py
+-rwxr-xr-x   0        0        0     1649 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test_yaml.py
+-rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 osm-fieldwork-0.3.1rc2/PKG-INFO
```

### Comparing `osm-fieldwork-0.3.1rc1/LICENSE.md` & `osm-fieldwork-0.3.1rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/README.md` & `osm-fieldwork-0.3.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/CSVDump.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/CSVDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/ODKDump.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/ODKForm.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKForm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/OdkCentral.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/OdkCentral.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             "form_update_mode": "match_exactly",
             "autosend": "wifi_and_cellular",
         }
         # If there is a config file with authentication setting, use that
         # so we don't have to supply this all the time. This is only used
         # when odk_client is used, and no parameters are passed in.
         if not self.url:
+            log.debug("Configuring ODKCentral from file .odkcentral")
             home = os.getenv("HOME")
             config = ".odkcentral"
             filespec = home + "/" + config
             if os.path.exists(filespec):
                 file = open(filespec, "r")
                 for line in file:
                     # Support embedded comments
@@ -86,17 +87,20 @@
                     if tmp[0] == "url":
                         self.url = tmp[1].strip("\n")
                     if tmp[0] == "user":
                         self.user = tmp[1].strip("\n")
                     if tmp[0] == "passwd":
                         self.passwd = tmp[1].strip("\n")
             else:
-                log.warning("You can put authentication settings in %s" % filespec)
+                log.warning(f"Authentication settings missing from {filespec}")
+        else:
+            log.debug(f"ODKCentral configuration parsed: {self.url}")
         # Base URL for the REST API
         self.version = "v1"
+        log.debug(f"Using {self.version} API")
         self.base = self.url + "/" + self.version + "/"
 
         # Authentication data
         self.auth = HTTPBasicAuth(self.user, self.passwd)
 
         # Use a persistant connect, better for multiple requests
         self.session = requests.Session()
@@ -139,26 +143,35 @@
         return projects
 
     def createProject(self,
                       name: str
                       ):
         """Create a new project on an ODK Central server if it doesn't
         already exist"""
+        log.debug(f"Checking if project named {name} exists already")
         exists = self.findProject(name)
         if exists:
-            log.debug(f"Project \"{name}\" already exists.")
+            log.debug(f"Project named {name} already exists.")
             return exists
         else:
             url = f"{self.base}projects"
-            result = self.session.post(
-                url, auth=self.auth, json={"name": name}, verify=self.verify
-            )
+            log.debug(f"POSTing project {name} to {url} with verify={self.verify}")
+            try:
+                result = self.session.post(
+                    url, auth=self.auth, json={"name": name}, verify=self.verify, timeout=4
+                )
+                result.raise_for_status()
+            except requests.exceptions.RequestException as e:
+                log.error(e)
+                log.error("Failed to submit to ODKCentral")
+            json_response = result.json()
+            log.debug(f"Returned: {json_response}")
             # update the internal list of projects
             self.listProjects()
-        return result.json()
+            return json_response
 
     def deleteProject(self,
                       project_id: int
                       ):
         """Delete a project on an ODK Central server"""
         url = f"{self.base}projects/{project_id}"
         self.session.delete(url, auth=self.auth, verify=self.verify)
@@ -502,33 +515,33 @@
                    draft: bool = False
                    ):
         """Create a new form on an ODK Central server"""
         if draft is not None:
             self.draft = draft
         headers = {"Content-Type": "application/xml"}
         if self.draft:
-            url = f"{self.base}projects/{projectId}/forms/{xmlFormId}/draft?ignoreWarnings=true&publish=false"
+            url = f"{self.base}projects/{projectId}/forms/{xform}/draft?ignoreWarnings=true&publish=false"
         else:
             url = f"{self.base}projects/{projectId}/forms?ignoreWarnings=true&publish=true"
 
         # Read the XML or XLS file
         file = open(filespec, "rb")
         xml = file.read()
         file.close()
         log.info("Read %d bytes from %s" % (len(xml), filespec))
 
         result = self.session.post(url, auth=self.auth,  data=xml, headers=headers, verify=self.verify)
         # epdb.st()
         # FIXME: should update self.forms with the new form
         if result.status_code != 200:
             if result.status_code == 409:
-                log.error(f"{xmlFormId} already exists on Central")
+                log.error(f"{xform} already exists on Central")
             else:
                 status = eval(result._content)
-                log.error(f"Couldn't create {xmlFormId} on Central: {status['message']}")
+                log.error(f"Couldn't create {xform} on Central: {status['message']}")
 
         return result.status_code
 
     def deleteForm(self,
                    projectId: int,
                    xform: str
                    ):
@@ -554,17 +567,17 @@
         else:
             xid = xform
 
         url = f"{self.base}projects/{projectId}/forms/{xid}/draft/publish?version={version}"
         result = self.session.post(url, auth=self.auth, verify=self.verify)
         if result.status_code != 200:
             status = eval(result._content)
-            log.error(f"Couldn't publish {xmlFormId} on Central: {status['message']}")
+            log.error(f"Couldn't publish {xform} on Central: {status['message']}")
         else:
-            log.info(f"Published {xmlFormId} on Central.")
+            log.info(f"Published {xform} on Central.")
         return result.status_code
 
     def dump(self):
         """Dump internal data structures, for debugging purposes only"""
         # super().dump()
         entries = len(self.media)
         print("Form has %d attachements" % entries)
```

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/basemapper.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/basemapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,20 @@
     base = args.outdir
 base = f"{base}/{args.source}tiles"
 
 if args.source:
     basemap = BaseMapper(args.boundary, base, args.source)
 else:
     logging.error("You need to specify a source!")
+    parser.print_help()
+    quit()
+
+if args.outfile is None:
+    logging.error("You need to specify an mbtiles or sqlitedb file!!")
+    parser.print_help()
     quit()
 
 outf = DataFile(args.outfile, basemap.getFormat())
 suffix = os.path.splitext(args.outfile)[1]
 if suffix == ".mbtiles":
     outf.addBounds(basemap.bbox)
 for level in zooms:
```

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/convert.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/convert.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/category.yaml` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/category.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/models.yaml` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/data_models/validate.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/validate.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/filter.yaml` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/filter.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/filter_data.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/filter_data.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/json2osm.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/json2osm.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,27 +20,30 @@
 
 import argparse
 import csv
 import os
 import logging
 import sys
 import json
+import geojson
 from sys import argv
 from osm_fieldwork.convert import Convert
 from osm_fieldwork.osmfile import OsmFile
 from osm_fieldwork.xlsforms import xlsforms_path
 from geojson import Point, Feature, FeatureCollection, dump
+from pathlib import Path
 #import pandas as pd
-#import re
+import math
+import re
 
 # set log level for urlib
 log = logging.getLogger(__name__)
 
 class JsonDump(Convert):
-    """A class to parse the CSV files from ODK Central"""
+    """A class to parse the JSON files from ODK Central or odk2geojson"""
 
     def __init__(self,
                  yaml: str = None
                  ):
         self.fields = dict()
         self.nodesets = dict()
         self.data = list()
@@ -50,14 +53,27 @@
         path = xlsforms_path.replace("xlsforms", "")
         if yaml:
             file = f"{path}{yaml}"
         else:
             file = f"{path}/xforms.yaml"
         self.config = super().__init__(yaml)
 
+        self.ignore = ('@id',
+                       '@xmlns:ev',
+                       '@xmlns:orx',
+                       '@xmlns:odk',
+                       '@xmlns:h',
+                       '@xmlns:jr',
+                       '@xmlns:xsd',
+                       'start',
+                       'end',
+                       'today',
+                       'meta',
+                       )
+
     # def parseXLS(self, xlsfile: str):
     #     """Parse the source XLSFile if available to look for details we need"""
     #     if xlsfile is not None and len(xlsfile) > 0:
     #         entries = pd.read_excel(xlsfile, sheet_name=[0])
     #         # There will only be a single sheet
     #         names = entries[0]['name']
     #         defaults = entries[0]['default']
@@ -77,15 +93,15 @@
 
     def createOSM(self,
                   filespec: str = "tmp.osm"
                   ):
         """Create an OSM XML output files"""
         log.debug("Creating OSM XML file: %s" % filespec)
         self.osm = OsmFile(filespec)
-        #self.osm.header()
+
     def writeOSM(self,
                  feature: dict
                  ):
         """Write a feature to an OSM XML output file"""
         out = ""
         if "id" in feature["tags"]:
             feature["id"] = feature["tags"]["id"]
@@ -115,118 +131,139 @@
             return None
         self.features.append(feature)
 
     def finishGeoJson(self):
         """Write the GeoJson FeatureCollection to the output file and close it"""
         features = list()
         for item in self.features:
+            #poi = Point()
             poi = Point((float(item["attrs"]["lon"]), float(item["attrs"]["lat"])))
             if "private" in item:
                 props = {**item["tags"], **item["private"]}
             else:
                 props = item["tags"]
             features.append(Feature(geometry=poi, properties=props))
         collection = FeatureCollection(features)
         dump(collection, self.json)
 
     def getAllTags(self,
                    data
                    ):
         all_tags = dict()
         tags = dict()
-        if type(data) == str:
-            return data
-        elif type(data) == dict:
+        if type(data) == dict:
             for k, v in data.items():
                 if type(v) == dict:
-                    log.info(f"Processing tag {k} = {v}")
+                    # log.debug(f"Processing tag {k} = {v}")
                     for k1, v1 in v.items():
+                        # log.debug(f"Processing sub tag {k} = {v}")
                         # tags.update(self.getAllTags(v))
                         if type(v1) == dict:
                             for i, j in v1.items():
                                 if type(j) == dict:
                                     # FIXME: this should handle more than one
-                                    # but so far I've only it be accuracy, no other
+                                    # but so far I've only it to be accuracy, no other
                                     # tags
                                     k2 = list(j.keys())[0]
                                     tags[k2] = list(j.values())[0]
                                 else:
                                     tags[i] = j
                         else:
                             tags[k1] = v1
-                    log.debug(f"TAGS: {tags}")
+                        # log.debug(f"TAGS: {tags}")
                 else:
                     if v:
                         # if k in self.saved:
                         #     if str(v) == 'nan' or len(v) == 0:
                         #         log.debug(f"FIXME: {k} {v}")
                         #         val = self.saved[k]
                         #         if val and len(v) == 0:
                         #             log.warning(f"Using last saved value for \"{k}\"! Now \"{val}\"" )
                         #             value = val
                         #         else:
                         #             self.saved[k] = value
                         #             log.debug(f"Updating last saved value for \"{k}\" with \"{value}\"")
-                        if type(v) == float:
+                        if type(v) != str:
                             tags[k] = str(v)
                         else:
                             tags[k] = v
                 all_tags.update(tags)
         return all_tags
 
     def parse(self,
               filespec: str,
               data: str = None
               ):
         """Parse the JSON file from ODK Central and convert it to a data structure"""
         all_tags = list()
         if not data:
-            f = open(filespec, newline="")
-            reader = json.load(f)
+            file = open(filespec, "r")
+            infile = Path(filespec)
+            if infile.suffix == ".geojson":
+                reader = geojson.load(file)
+            elif infile.suffix == ".json":
+                reader = json.load(file)
+            else:
+                log.error("Need to specify a JSON or GeoJson file!")
+                return all_tags
         else:
-            reader = json.loads(data)
+            reader = geojson.loads(data)
         
         total = list()
-        for row in reader['value']:
+        # JSON files from Central use value as the keyword, whereas
+        # GeoJSON uses features for the same thing.
+        if 'value' in reader:
+            data = reader['value']
+        elif 'features' in reader:
+            data = reader['features']
+        for row in data:
             # log.info(f"ROW: {row}")
             tags = dict()
-            for keyword, value in row.items():
+            if 'geometry' in row:
+                tags['geometry'] = row['geometry']
+            if 'properties' in row:
+                indata = row['properties'] # A GeoJson formatted file
+            else:
+                indata = row    # A JOSM file from ODK Central
+            for keyword, value in indata.items():
                 # There's many extraneous fields in the input file which we don't need.
                 base = keyword.lower()
                 if (
                     base is None
                     or base in self.ignore
                     or value is None
                     or len(value) == 0
                 ):
                     continue
                 if keyword is None or len(keyword) == 0:
                     continue
-                alltags = self.getAllTags(value)
-                print(f"FIXME3: {alltags}")
-                for k, v in alltags.items():
-                    if k in self.ignore:
-                        continue
-                    if v:
-                        items = dict()
-                        if type(v) == dict:
-                            v1 = alltags[k]
-                            if len(v1) > 1:
-                                log.warning("Got more than 1 result! {v1}")
-                                v2 = v1[v1.keys()]
-                                items = self.convertEntry(k, v2)
-                        else:
-                            items = self.convertEntry(k, v)
-                        #    for entry in items:
-                        #        for k, v in entry.items():
-                        #            tags[k] = v
-                        #    else:
-                        #tags[k1] = v1
+                if type(value) == str:
+                    items = self.convertEntry(keyword, value)
+                    tags.update(items)
+                else:
+                    alltags = self.getAllTags(value)
+                    for k, v in alltags.items():
+                        # if k in self.ignore:
+                        #     continue
+                        if v:
+                            items = dict()
+                            if type(v) == dict:
+                                v1 = alltags[k]
+                                if len(v1) > 1:
+                                    log.warning("Got more than 1 result! {v1}")
+                                    v2 = v1[v1.keys()]
+                                    items = self.convertEntry(k, v2)
+                            else:
+                                items = self.convertEntry(k, v)
+                                #    for entry in items:
+                                #        for k, v in entry.items():
+                                #            tags[k] = v
+                                #    else:
+                                #tags[k1] = v1
                         tags.update(items)
-            log.debug(f"\tFIXME1: {tags}")
             total.append(tags)
         return total
 
     def createEntry(self,
                     entry: dict
                     ):
         """Create the feature data structure"""
@@ -248,19 +285,42 @@
                 "uid",
                 "user",
                 "version",
                 "action",
             )
             # When using existing OSM data, there's a special geometry field.
             # Otherwise use the GPS coordinates where you are.
+            lat = None
+            lon = None
+            if type(value) == float:
+                continue
             if key == "geometry":
-                if value and len(value) == 3:
-                    attrs["lat"] = value[1]
-                    attrs["lon"] = value[0]
-                    continue
+                # The GeoJson file has the geometry field. Usually it's a dict
+                # but on occasion it's a string instead, so turn it into a list
+                # log.debug(f"FIXME: {value} {type(value)}")
+                if type(value) == str:
+                    if value[0] ==  '[':
+                        coords = eval(value)
+                        lat = coords[1]
+                        lon = coords[0]
+                    else:
+                        coords = value.split(' ')
+                        lat = coords[0]
+                        lon = coords[1]
+                    # log.debug(f"VALUE STRING: {coords}")
+                elif type(value) == geojson.geometry.Point:
+                    lat = value['coordinates'][1]
+                    lon = value['coordinates'][0]
+                    # log.debug(f"VALUE POINT: {lat}/{lon}")
+                elif type(value) == list:
+                    lat = float(value[1])
+                    lon = float(value[0])
+                attrs["lat"] = lat
+                attrs["lon"] = lon
+                # log.debug(f"ATTRS: {attrs}")
 
             if key is not None and len(key) > 0 and key in attributes:
                 attrs[key] = value
                 log.debug("Adding attribute %s with value %s" % (key, value))
             else:
                 if key in self.multiple:
                     for item in value:
@@ -281,27 +341,29 @@
                         log.debug("Adding reference %s" % tag)
                     elif len(str(value)) > 0:
                         if self.privateData(key):
                             priv[key] = value
                         else:
                             tags[key] = value
             if len(tags) > 0:
+                if 'geometry' in tags:
+                    del tags['geometry']
                 feature["attrs"] = attrs
                 feature["tags"] = tags
             if len(refs) > 0:
                 feature["refs"] = refs
             if len(priv) > 0:
                 feature["private"] = priv
 
         return feature
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
-        description="convert CSV from ODK Central to OSM XML"
+        description="convert JSON from ODK Central to OSM XML"
     )
     parser.add_argument("-v", "--verbose", action="store_true", help="verbose output")
     parser.add_argument("-y", "--yaml", help="Alternate YAML file")
     parser.add_argument("-x", "--xlsfile", help="Source XLSFile")
     parser.add_argument(
         "-i", "--infile", help="The input file downloaded from ODK Central"
     )
@@ -320,35 +382,48 @@
         ch.setFormatter(formatter)
         root.addHandler(ch)
 
     if args.yaml:
         jsonin = JsonDump(args.yaml)
     else:
         jsonin = JsonDump()
-    # jsonin.parseXLS(args.xlsfile)    
-    osmoutfile = os.path.basename(args.infile.replace(".json", ".osm"))
+    # jsonin.parseXLS(args.xlsfile)
+
+    # Modify the input file name for the 2 output files, which will get written
+    # to the current directory.
+    infile = Path(args.infile)
+    base = os.path.splitext(infile.name)[0]
+    osmoutfile = f"{base}-out.osm"
     jsonin.createOSM(osmoutfile)
 
-    jsonoutfile = os.path.basename(args.infile.replace(".json", ".geojson"))
+    jsonoutfile = f"{base}-out.geojson"
     jsonin.createGeoJson(jsonoutfile)
 
-    log.debug("Parsing csv files %r" % args.infile)
-    data = jsonin.parse(args.infile)
+    log.debug("Parsing JSON file %r" % args.infile)
+    data = jsonin.parse(infile.as_posix())
     # This OSM XML file only has OSM appropriate tags and values
     for entry in data:
         feature = jsonin.createEntry(entry)
         # Sometimes bad entries, usually from debugging XForm design, sneak in
         if len(feature) == 0:
             continue
         if len(feature) > 0:
             if "lat" not in feature["attrs"]:
-                log.warning("Bad record! %r" % feature)
-                continue
+                if 'geometry' in feature['tags']:
+                    if type(feature['tags']['geometry']) == str:
+                        coords = list(feature['tags']['geometry'])
+                        # del feature['tags']['geometry']
+                    else:
+                        coords = feature['tags']['geometry']['coordinates']
+                        # del feature['tags']['geometry']
+                    feature['attrs'] = {'lat': coords[1], 'lon': coords[0]}
+                else:
+                    log.warning("Bad record! %r" % feature)
+                    continue
             jsonin.writeOSM(feature)
             # This GeoJson file has all the data values
             jsonin.writeGeoJson(feature)
-            # print("TAGS: %r" % feature['tags'])
 
     jsonin.finishOSM()
     jsonin.finishGeoJson()
     log.info("Wrote OSM XML file: %r" % osmoutfile)
     log.info("Wrote GeoJson file: %r" % jsonoutfile)
```

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/make_data_extract.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/make_data_extract.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/odk2csv.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/odk2csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/odk_client.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/odk_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
             "There are %d submissions for XForm %s" % (len(submissions), args.form)
         )
         for file in submissions:
             form.submissions.append(file)
             print("%s: %s" % (file["instanceId"], file["createdAt"]))
 
     elif args.xform == "json":
-        submissions = form.getSubmissions(args.id, args.form, True, True)
+        submissions = form.getSubmissions(args.id, args.form, False, True, True)
         logging.info(
             "There are %d submissions for XForm %s" % (len(submissions), args.form)
         )
         for file in submissions:
             form.submissions.append(file)
             #print("%s: %s" % (file["instanceId"], file["createdAt"]))
```

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/odk_merge.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/odk_merge.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/osmfile.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/osmfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 
     def isclosed(self):
         return self.file.closed
 
     def header(self):
         if self.file is not False:
             self.file.write("<?xml version='1.0' encoding='UTF-8'?>\n")
-            # self.file.write('<osm version="0.6" generator="gosm 0.1" timestamp="2017-03-13T21:43:02Z">\n')
-            self.file.write('<osm version="0.6" generator="gosm 0.1">\n')
+            # self.file.write('<osm version="0.6" generator="osm-fieldowrk 0.3" timestamp="2017-03-13T21:43:02Z">\n')
+            self.file.write('<osm version="0.6" generator="osm-fieldwork 0.3">\n')
             self.file.flush()
 
     def footer(self):
         # logging.debug("FIXME: %r" % self.file)
         self.file.write("</osm>\n")
         self.file.flush()
         if self.file is False:
```

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/sqlite.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/sqlite.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xforms.yaml` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xforms.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,14 @@
   - formVersion
   - edits
   - attachmentsexpected
   - attachmentspresent
   - reviewstate
   - edits
   - gps_type
-  - accuracy
   - deviceid
   - key
   - start
   - end
   - today
   - status
   - instanceid
```

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/Makefile` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/Makefile`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/__init__.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/amenities.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/amenities.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/buildings.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/buildings.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/camping.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/camping.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/cemeteries.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/cemeteries.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/education.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/education.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/health.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/health.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/historical.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/historical.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/hotspring.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/hotspring.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/landusage.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/landusage.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/landuse.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/landuse.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/amenities.csv` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/amenities.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/lib/towns.csv` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/towns.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/nature.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/nature.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/places.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/places.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/religious.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/religious.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/slides.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/slides.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/solidwaste.xlsx` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/solidwaste.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/toilets.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/toilets.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/transportation.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/transportation.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/waste_collection.xlsx` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waste_collection.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/wastedisposal.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/wastedisposal.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/waterpoints.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waterpoints.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/xlsforms/waterways.xls` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waterways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/osm_fieldwork/yamlfile.py` & `osm-fieldwork-0.3.1rc2/osm_fieldwork/yamlfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/pyproject.toml` & `osm-fieldwork-0.3.1rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 classifiers = [
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering :: GIS",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
 ]
-version = "0.3.1rc1"
+version = "0.3.1rc2"
 
 [project.urls]
 homepage = "https://github.com/hotosm/osm-fieldwork/wiki"
 documentation = "https://github.com/hotosm/osm-fieldwork/wiki"
 repository = "https://github.com/hotosm/osm-fieldwork"
 
 [project.optional-dependencies]
@@ -68,15 +68,15 @@
 testpaths = [
     "tests",
 ]
 pythonpath = "osm_fieldwork"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.1rc1"
+version = "0.3.1rc2"
 version_files = [
     "pyproject.toml:version",
     "osm_fieldwork/__version__.py",
     "Makefile:VERSION",
 ]
 
 [build-system]
```

### Comparing `osm-fieldwork-0.3.1rc1/tests/Test.yaml` & `osm-fieldwork-0.3.1rc2/tests/Test.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/tests/test.csv` & `osm-fieldwork-0.3.1rc2/tests/test.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/tests/test_convert.py` & `osm-fieldwork-0.3.1rc2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/tests/test_csv.py` & `osm-fieldwork-0.3.1rc2/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/tests/test_osm.py` & `osm-fieldwork-0.3.1rc2/tests/test_osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/tests/test_yaml.py` & `osm-fieldwork-0.3.1rc2/tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc1/PKG-INFO` & `osm-fieldwork-0.3.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-fieldwork
-Version: 0.3.1rc1
+Version: 0.3.1rc2
 Summary: Convert CSV files from ODK Central to OSM format.
 License: GPL-3.0-only
 Keywords: fmtm,odk,hot,openstreetmap,opendatakit
 Author-email: Rob Savoye <rob.savoye@hotosm.org>
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

