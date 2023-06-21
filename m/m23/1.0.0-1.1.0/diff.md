# Comparing `tmp/m23-1.0.0.tar.gz` & `tmp/m23-1.1.0.tar.gz`

## Comparing `m23-1.0.0.tar` & `m23-1.1.0.tar`

### file list

```diff
@@ -1,69 +1,68 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 m23-1.0.0/.DS_Store
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.0.0/.flake8
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 m23-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 m23-1.0.0/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.0.0/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.0.0/nights_csv.toml
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 m23-1.0.0/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.0.0/renormalize.toml
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 m23-1.0.0/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.0.0/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 m23-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/matrix/utils.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/__init__.py
--rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    22058 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725365 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/reference/README.md
--rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/reference/ref_revised_71.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/trans/fits.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.0.0/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 m23-1.0.0/.gitignore
--rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 m23-1.0.0/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 m23-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12531 2020-02-02 00:00:00.000000 m23-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.1.0/.flake8
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 m23-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.1.0/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.1.0/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.1.0/nights_csv.toml
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.1.0/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.1.0/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.1.0/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 m23-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    22118 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725365 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/reference/README.md
+-rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/reference/ref_revised_71.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.1.0/.gitignore
+-rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 m23-1.1.0/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13681 2020-02-02 00:00:00.000000 m23-1.1.0/PKG-INFO
```

### Comparing `m23-1.0.0/brown.toml` & `m23-1.1.0/brown.toml`

 * *Files 24% similar despite different names*

```diff
@@ -35,7 +35,10 @@
     [[input.nights]]
     path = "F://Summer 2019/September 8, 2019"
     # Because we haven't provided masterflat, this night must have flats to use 
     
 
 [output]
 path = "C://Data Processing/2019 Python Processed"
+# The options below are optional and default to false if not specified
+save_aligned = false
+save_calibrated = false
```

### Comparing `m23-1.0.0/mf.toml` & `m23-1.1.0/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/nights_csv.toml` & `m23-1.1.0/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/rainbow.toml` & `m23-1.1.0/rainbow.toml`

 * *Files 13% similar despite different names*

```diff
@@ -40,8 +40,11 @@
 
     [[input.nights]]
     path = "F://Summer 2022/September 8, 2022"
     # Because we haven't provided masterflat, this night must have flats to use 
 
 
 [output]
-path = "D://xxx"
+path = "D://xxx"
+# The options below are optional and default to false if not specified
+save_aligned = false
+save_calibrated = false
```

### Comparing `m23-1.0.0/requirements.txt` & `m23-1.1.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,25 +15,20 @@
 ephem==4.1.4
 exceptiongroup==1.1.1
 fonttools==4.38.0
 gitdb==4.0.10
 GitPython==3.1.31
 idna==3.4
 imageio==2.25.0
-<<<<<<< HEAD
 importlib-metadata==6.7.0
 iniconfig==2.0.0
 invoke==2.1.3
 jaraco.classes==3.2.3
 keyring==24.0.0
-=======
-iniconfig==2.0.0
->>>>>>> a5f0cd98cbe73e0ae673fd67355f8c969f502f0e
 kiwisolver==1.4.4
-m23 @ file:///Users/suman/Desktop/astro/m23
 matplotlib==3.7.0
 more-itertools==9.1.0
 mypy-extensions==1.0.0
 networkx==3.0
 numpy==1.24.2
 opencv-python==4.7.0.68
 packaging==23.0
@@ -41,18 +36,14 @@
 Pillow==9.4.0
 pkginfo==1.9.6
 platformdirs==3.0.0
 pluggy==1.0.0
 pyerfa==2.0.0.1
 Pygments==2.15.1
 pyparsing==3.0.9
-<<<<<<< HEAD
-pyproject_hooks==1.0.0
-=======
->>>>>>> a5f0cd98cbe73e0ae673fd67355f8c969f502f0e
 pytest==7.3.2
 python-dateutil==2.8.2
 python-gitlab==3.15.0
 python-semantic-release==7.34.6
 PyWavelets==1.4.1
 PyYAML==6.0
 readme-renderer==40.0
```

### Comparing `m23-1.0.0/.github/workflows/python-publish.yml` & `m23-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/.vscode/settings.json` & `m23-1.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/__main__.py` & `m23-1.1.0/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/constants.py` & `m23-1.1.0/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/align/__init__.py` & `m23-1.1.0/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/calibrate/calibration.py` & `m23-1.1.0/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/calibrate/master_calibrate.py` & `m23-1.1.0/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/charts/__init__.py` & `m23-1.1.0/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/combine/__init__.py` & `m23-1.1.0/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/extract/__init__.py` & `m23-1.1.0/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/__init__.py` & `m23-1.1.0/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/aligned_combined_file.py` & `m23-1.1.0/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/alignment_stats_file.py` & `m23-1.1.0/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/color_normalized_file.py` & `m23-1.1.0/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/flux_log_combined_file.py` & `m23-1.1.0/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/log_file_combined_file.py` & `m23-1.1.0/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/masterflat_file.py` & `m23-1.1.0/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/normfactor_file.py` & `m23-1.1.0/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/raw_image_file.py` & `m23-1.1.0/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/reference_log_file.py` & `m23-1.1.0/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/ri_color_file.py` & `m23-1.1.0/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/file/sky_bg_file.py` & `m23-1.1.0/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/internight_normalize/__init__.py` & `m23-1.1.0/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/matrix/fill.py` & `m23-1.1.0/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/norm/__init__.py` & `m23-1.1.0/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/norm/get_line.py` & `m23-1.1.0/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/processor/config_loader.py` & `m23-1.1.0/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/processor/generate_masterflat.py` & `m23-1.1.0/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.1.0/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/processor/nights_csv.py` & `m23-1.1.0/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/processor/nights_csv_config_loader.py` & `m23-1.1.0/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/processor/process_nights.py` & `m23-1.1.0/src/m23/processor/process_nights.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from typing import Iterable, List
 
 import numpy as np
 import toml
 from astropy.io.fits import getdata
 
+from m23 import __version__
 from m23.align import image_alignment
 from m23.calibrate.calibration import calibrateImages
 from m23.calibrate.master_calibrate import makeMasterDark, makeMasterFlat
 from m23.charts import draw_normfactors_chart
 from m23.constants import (
     ALIGNED_COMBINED_FOLDER_NAME,
     ALIGNED_FOLDER_NAME,
@@ -263,15 +264,15 @@
     ch = logging.FileHandler(log_file_path)
     ch.setFormatter(formatter)
     logger.addHandler(ch)
     # Write to std out in addition to writing to a logfile
     ch2 = logging.StreamHandler(sys.stdout)
     ch2.setFormatter(formatter)
     logger.addHandler(ch2)  # Write to stdout
-    logger.info(f"Starting processing for {night_date}")
+    logger.info(f"Starting processing for {night_date} with m23 version: {__version__}")
 
     ref_image_path = config["reference"]["image"]
     ref_file_path = config["reference"]["file"]
     color_ref_file_path = config["reference"]["color"]
 
     save_aligned_images = config["output"]["save_aligned"]
     save_calibrated_images = config["output"]["save_calibrated"]
```

### Comparing `m23-1.0.0/src/m23/processor/renormalize.py` & `m23-1.1.0/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/processor/renormalize_config_loader.py` & `m23-1.1.0/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.1.0/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/reference/MeanRI100.txt` & `m23-1.1.0/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/reference/README.md` & `m23-1.1.0/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/reference/ref_revised_71.txt` & `m23-1.1.0/src/m23/reference/ref_revised_71.txt`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/sky/__init__.py` & `m23-1.1.0/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/sky/moon/__init__.py` & `m23-1.1.0/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/utils/__init__.py` & `m23-1.1.0/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/utils/date.py` & `m23-1.1.0/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/src/m23/utils/rename.py` & `m23-1.1.0/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.0.0/.gitignore` & `m23-1.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -181,7 +181,9 @@
 
 test*.py
 docs
 
 !tests/**
 
 idea/*
+
+tests/__pycache__
```

### Comparing `m23-1.0.0/README.md` & `m23-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,17 @@
     [[input.nights]]
     path = "F://Summer 2019/September 8, 2019"
     # Because we haven't provided masterflat, this night must have flats to use
 
 
 [output]
 path = "C://Data Processing/2019 Python Processed"
+# The options below are optional and default to false if not specified
+save_aligned = false
+save_calibrated = false
 
 ```
 
 The file should be pretty self explanatory. Note that `#` denotes the beginning end of line comment.
 Still few things to note:
 
 1. Provide masterflat for only those nights where we would like to use masterflat of other nights.
@@ -262,7 +265,26 @@
 `pip install .` in your terminal form the root directory of project. Then invoke
 the tests by running merely `pytest`. You should have already run `pip install -
 r requirements.txt` before running the tests.
 
 ### Contributing
 
 This library has bugs, like most software and needs your valuable contribution.
+This project uses semantic versioning meaning that the version names are
+determined based on the work automatically rather than the author manually
+changing them. We use [python semantic
+release](https://python-semantic-release.readthedocs.io/en/latest/) for that.
+All you need to do is to write commit messages in a certain format, and the
+releases will be created automatically for you by the github actions and those
+releases published to github release as well as pypi. Navigate to the github
+actions tab to check the status of your release or if something failed. Your
+commit message must be followed by one of the few special keywords:
+
+1. "chore" for chore tasks
+1. "docs" for documentation related commits
+1. "feat" for new feature
+1. "fix" for bugfix
+
+Note that if any of your commits make breaking changes, your commit message must
+also contain the phrase "BREAKING CHANGE". This will trigger a major version
+update. See some of the previous commit messages for more information and feel
+free too ask if you have confusion.
```

### Comparing `m23-1.0.0/PKG-INFO` & `m23-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.0.0
+Version: 1.1.0
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: numpy==1.24.2
 Requires-Dist: opencv-python==4.7.0.68
@@ -94,14 +94,17 @@
     [[input.nights]]
     path = "F://Summer 2019/September 8, 2019"
     # Because we haven't provided masterflat, this night must have flats to use
 
 
 [output]
 path = "C://Data Processing/2019 Python Processed"
+# The options below are optional and default to false if not specified
+save_aligned = false
+save_calibrated = false
 
 ```
 
 The file should be pretty self explanatory. Note that `#` denotes the beginning end of line comment.
 Still few things to note:
 
 1. Provide masterflat for only those nights where we would like to use masterflat of other nights.
@@ -276,7 +279,26 @@
 `pip install .` in your terminal form the root directory of project. Then invoke
 the tests by running merely `pytest`. You should have already run `pip install -
 r requirements.txt` before running the tests.
 
 ### Contributing
 
 This library has bugs, like most software and needs your valuable contribution.
+This project uses semantic versioning meaning that the version names are
+determined based on the work automatically rather than the author manually
+changing them. We use [python semantic
+release](https://python-semantic-release.readthedocs.io/en/latest/) for that.
+All you need to do is to write commit messages in a certain format, and the
+releases will be created automatically for you by the github actions and those
+releases published to github release as well as pypi. Navigate to the github
+actions tab to check the status of your release or if something failed. Your
+commit message must be followed by one of the few special keywords:
+
+1. "chore" for chore tasks
+1. "docs" for documentation related commits
+1. "feat" for new feature
+1. "fix" for bugfix
+
+Note that if any of your commits make breaking changes, your commit message must
+also contain the phrase "BREAKING CHANGE". This will trigger a major version
+update. See some of the previous commit messages for more information and feel
+free too ask if you have confusion.
```

