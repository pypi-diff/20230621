# Comparing `tmp/wahoomc-4.0.3a0.tar.gz` & `tmp/wahoomc-4.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wahoomc-4.0.3a0.tar", last modified: Sun Jun  4 19:25:45 2023, max compression
+gzip compressed data, was "wahoomc-4.0.3a1.tar", last modified: Wed Jun 21 14:17:36 2023, max compression
```

## Comparing `wahoomc-4.0.3a0.tar` & `wahoomc-4.0.3a1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.374887 wahoomc-4.0.3a0/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4403 2023-06-04 19:25:45.375048 wahoomc-4.0.3a0/PKG-INFO
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3862 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/README.md
--rw-r--r--   0 bkreusc  (1890165452) 58041779      103 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/pyproject.toml
--rw-r--r--   0 bkreusc  (1890165452) 58041779      829 2023-06-04 19:25:45.376099 wahoomc-4.0.3a0/setup.cfg
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.351466 wahoomc-4.0.3a0/tests/
--rw-r--r--   0 bkreusc  (1890165452) 58041779      812 2022-10-06 21:14:05.000000 wahoomc-4.0.3a0/tests/test_cli.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6758 2023-06-04 19:22:17.000000 wahoomc-4.0.3a0/tests/test_constants.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     5494 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_constants_geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     7030 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_downloader.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    10238 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_generated_files.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     9487 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     7214 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_osm_maps.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3514 2023-03-27 20:10:10.000000 wahoomc-4.0.3a0/tests/test_setup.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.355392 wahoomc-4.0.3a0/wahoomc/
--rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/__init__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779      131 2023-03-27 20:10:10.000000 wahoomc-4.0.3a0/wahoomc/__main__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     1592 2023-06-04 19:25:01.000000 wahoomc-4.0.3a0/wahoomc/constants.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4597 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/constants_functions.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    12209 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/downloader.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     5720 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/file_directory_functions.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    21372 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4635 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/geofabrik_json.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.356645 wahoomc-4.0.3a0/wahoomc/init/
--rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2023-03-27 20:10:10.000000 wahoomc-4.0.3a0/wahoomc/init/__init__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779      137 2023-03-27 20:10:10.000000 wahoomc-4.0.3a0/wahoomc/init/__main__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    18039 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/input.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3668 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/main.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    39982 2023-06-04 19:22:20.000000 wahoomc-4.0.3a0/wahoomc/osm_maps_functions.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.358095 wahoomc-4.0.3a0/wahoomc/resources/
--rw-r--r--   0 bkreusc  (1890165452) 58041779      824 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/resources/sea.osm
--rw-r--r--   0 bkreusc  (1890165452) 58041779    15766 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/resources/shape2osm.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.358660 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     9834 2023-06-04 19:22:17.000000 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779    41694 2022-10-09 22:58:21.000000 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.359686 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_initial/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6354 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779     2360 2023-06-04 19:22:17.000000 wahoomc-4.0.3a0/wahoomc/resources/tags-to-keep.json
--rw-r--r--   0 bkreusc  (1890165452) 58041779      511 2023-03-27 20:10:11.000000 wahoomc-4.0.3a0/wahoomc/resources/tunnel-transform.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779    10562 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/setup_functions.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.374011 wahoomc-4.0.3a0/wahoomc/tooling_win/
--rw-r--r--   0 bkreusc  (1890165452) 58041779   269312 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/7za.dll
--rw-r--r--   0 bkreusc  (1890165452) 58041779   739840 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/7za.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   158720 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/7zxa.dll
--rw-r--r--   0 bkreusc  (1890165452) 58041779   108544 2022-05-21 18:01:36.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/lzma.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   299998 2022-11-29 06:53:00.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/osmconvert.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   311997 2022-11-29 06:53:00.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/osmconvert64-0.8.8p.exe
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.356275 wahoomc-4.0.3a0/wahoomc.egg-info/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4403 2023-06-04 19:25:45.000000 wahoomc-4.0.3a0/wahoomc.egg-info/PKG-INFO
--rw-r--r--   0 bkreusc  (1890165452) 58041779     1183 2023-06-04 19:25:45.000000 wahoomc-4.0.3a0/wahoomc.egg-info/SOURCES.txt
--rw-r--r--   0 bkreusc  (1890165452) 58041779        1 2023-06-04 19:25:45.000000 wahoomc-4.0.3a0/wahoomc.egg-info/dependency_links.txt
--rw-r--r--   0 bkreusc  (1890165452) 58041779        8 2023-06-04 19:25:45.000000 wahoomc-4.0.3a0/wahoomc.egg-info/top_level.txt
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.637538 wahoomc-4.0.3a1/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4403 2023-06-21 14:17:36.637784 wahoomc-4.0.3a1/PKG-INFO
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3862 2023-06-15 20:15:57.000000 wahoomc-4.0.3a1/README.md
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      103 2022-05-21 18:01:35.000000 wahoomc-4.0.3a1/pyproject.toml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      829 2023-06-21 14:17:36.638238 wahoomc-4.0.3a1/setup.cfg
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.620452 wahoomc-4.0.3a1/tests/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      812 2022-10-06 21:14:05.000000 wahoomc-4.0.3a1/tests/test_cli.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6758 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/tests/test_constants.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     5494 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/tests/test_constants_geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     7030 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/tests/test_downloader.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    10238 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/tests/test_generated_files.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     9487 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/tests/test_geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     7214 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/tests/test_osm_maps.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3514 2023-03-27 20:10:10.000000 wahoomc-4.0.3a1/tests/test_setup.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.624149 wahoomc-4.0.3a1/wahoomc/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2022-05-21 18:01:35.000000 wahoomc-4.0.3a1/wahoomc/__init__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      131 2023-03-27 20:10:10.000000 wahoomc-4.0.3a1/wahoomc/__main__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     1592 2023-06-21 14:17:02.000000 wahoomc-4.0.3a1/wahoomc/constants.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4597 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/wahoomc/constants_functions.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    12209 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/wahoomc/downloader.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     5720 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/wahoomc/file_directory_functions.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    21372 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/wahoomc/geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4635 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/wahoomc/geofabrik_json.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.625741 wahoomc-4.0.3a1/wahoomc/init/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2023-03-27 20:10:10.000000 wahoomc-4.0.3a1/wahoomc/init/__init__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      137 2023-03-27 20:10:10.000000 wahoomc-4.0.3a1/wahoomc/init/__main__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    18039 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/wahoomc/input.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3668 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/wahoomc/main.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    39985 2023-06-21 13:01:56.000000 wahoomc-4.0.3a1/wahoomc/osm_maps_functions.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.627017 wahoomc-4.0.3a1/wahoomc/resources/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      824 2022-05-21 18:01:35.000000 wahoomc-4.0.3a1/wahoomc/resources/sea.osm
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    15766 2022-05-21 18:01:35.000000 wahoomc-4.0.3a1/wahoomc/resources/shape2osm.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.627666 wahoomc-4.0.3a1/wahoomc/resources/tag_wahoo_adjusted/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     9834 2023-06-19 20:32:18.000000 wahoomc-4.0.3a1/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    41694 2022-10-09 22:58:21.000000 wahoomc-4.0.3a1/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.628207 wahoomc-4.0.3a1/wahoomc/resources/tag_wahoo_initial/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6354 2022-05-21 18:01:35.000000 wahoomc-4.0.3a1/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     2360 2023-06-19 20:32:18.000000 wahoomc-4.0.3a1/wahoomc/resources/tags-to-keep.json
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      511 2023-06-06 15:43:56.000000 wahoomc-4.0.3a1/wahoomc/resources/tunnel-transform.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    10562 2023-06-21 13:01:56.000000 wahoomc-4.0.3a1/wahoomc/setup_functions.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.636745 wahoomc-4.0.3a1/wahoomc/tooling_win/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   269312 2022-05-21 18:01:35.000000 wahoomc-4.0.3a1/wahoomc/tooling_win/7za.dll
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   739840 2022-05-21 18:01:35.000000 wahoomc-4.0.3a1/wahoomc/tooling_win/7za.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   158720 2022-05-21 18:01:35.000000 wahoomc-4.0.3a1/wahoomc/tooling_win/7zxa.dll
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   108544 2022-05-21 18:01:36.000000 wahoomc-4.0.3a1/wahoomc/tooling_win/lzma.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   299998 2022-11-29 06:53:00.000000 wahoomc-4.0.3a1/wahoomc/tooling_win/osmconvert.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   311997 2022-11-29 06:53:00.000000 wahoomc-4.0.3a1/wahoomc/tooling_win/osmconvert64-0.8.8p.exe
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-21 14:17:36.625429 wahoomc-4.0.3a1/wahoomc.egg-info/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4403 2023-06-21 14:17:36.000000 wahoomc-4.0.3a1/wahoomc.egg-info/PKG-INFO
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     1183 2023-06-21 14:17:36.000000 wahoomc-4.0.3a1/wahoomc.egg-info/SOURCES.txt
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        1 2023-06-21 14:17:36.000000 wahoomc-4.0.3a1/wahoomc.egg-info/dependency_links.txt
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        8 2023-06-21 14:17:36.000000 wahoomc-4.0.3a1/wahoomc.egg-info/top_level.txt
```

### Comparing `wahoomc-4.0.3a0/PKG-INFO` & `wahoomc-4.0.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wahoomc
-Version: 4.0.3a0
+Version: 4.0.3a1
 Summary: Create maps for your Wahoo bike computer based on latest OSM maps
 Home-page: https://github.com/treee111/wahooMapsCreator
 Author: Benjamin Kreuscher
 Author-email: benni.kreuscher@gmail.com
 Project-URL: Bug Tracker, https://github.com/treee111/wahooMapsCreator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wahoomc Version: 4.0.3a0 Summary: Create maps for
+Metadata-Version: 2.1 Name: wahoomc Version: 4.0.3a1 Summary: Create maps for
 your Wahoo bike computer based on latest OSM maps Home-page: https://
 github.com/treee111/wahooMapsCreator Author: Benjamin Kreuscher Author-email:
 benni.kreuscher@gmail.com Project-URL: Bug Tracker, https://github.com/
 treee111/wahooMapsCreator/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.10 Description-Content-Type:
 text/markdown
```

### Comparing `wahoomc-4.0.3a0/README.md` & `wahoomc-4.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/setup.cfg` & `wahoomc-4.0.3a1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wahoomc
-version = 4.0.3a0
+version = 4.0.3a1
 author = Benjamin Kreuscher
 author_email = benni.kreuscher@gmail.com
 description = Create maps for your Wahoo bike computer based on latest OSM maps
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/treee111/wahooMapsCreator
 project_urls =
```

### Comparing `wahoomc-4.0.3a0/tests/test_cli.py` & `wahoomc-4.0.3a1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/tests/test_constants.py` & `wahoomc-4.0.3a1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/tests/test_constants_geofabrik.py` & `wahoomc-4.0.3a1/tests/test_constants_geofabrik.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/tests/test_downloader.py` & `wahoomc-4.0.3a1/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/tests/test_generated_files.py` & `wahoomc-4.0.3a1/tests/test_generated_files.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/tests/test_geofabrik.py` & `wahoomc-4.0.3a1/tests/test_geofabrik.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/tests/test_osm_maps.py` & `wahoomc-4.0.3a1/tests/test_osm_maps.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/tests/test_setup.py` & `wahoomc-4.0.3a1/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/constants.py` & `wahoomc-4.0.3a1/wahoomc/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # Python Package - wahooMapsCreator directory
 WAHOO_MC_DIR = os.path.dirname(__file__)
 RESOURCES_DIR = os.path.join(WAHOO_MC_DIR, 'resources')
 TOOLING_WIN_DIR = os.path.join(WAHOO_MC_DIR, 'tooling_win')
 # location of repo / python installation - not used
 ROOT_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir))
-VERSION = '4.0.3a0'
+VERSION = '4.0.3a1'
 
 
 block_download = ['dach', 'alps', 'britain-and-ireland', 'south-africa-and-lesotho',
                   'us-midwest', 'us-northeast', 'us-pacific', 'us-south', 'us-west']
 
 # Special_regions like (former) colonies where the map of the wanted region is not present in the map of the parent country.
 # example Guadeloupe, it's Geofabrik parent country is France but Guadeloupe is not located within the region covered by the map of France.
```

### Comparing `wahoomc-4.0.3a0/wahoomc/constants_functions.py` & `wahoomc-4.0.3a1/wahoomc/constants_functions.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/downloader.py` & `wahoomc-4.0.3a1/wahoomc/downloader.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/file_directory_functions.py` & `wahoomc-4.0.3a1/wahoomc/file_directory_functions.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/geofabrik.py` & `wahoomc-4.0.3a1/wahoomc/geofabrik.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/geofabrik_json.py` & `wahoomc-4.0.3a1/wahoomc/geofabrik_json.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/input.py` & `wahoomc-4.0.3a1/wahoomc/input.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/main.py` & `wahoomc-4.0.3a1/wahoomc/main.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/osm_maps_functions.py` & `wahoomc-4.0.3a1/wahoomc/osm_maps_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,20 @@
 
 def run_subprocess_and_log_output(cmd, error_message, cwd=""):
     """
     run given cmd-subprocess and issue error message if wished
     """
     if not cwd:
         process = subprocess.run(
-            cmd, capture_output=True, text=True, encoding="utf-8", check=True)
+            cmd, capture_output=True, text=True, encoding="utf-8", check=False)
 
     else:
         process = subprocess.run(  # pylint: disable=consider-using-with
-            cmd, capture_output=True, cwd=cwd, text=True, encoding="utf-8", check=True)
+            cmd, capture_output=True, cwd=cwd, text=True, encoding="utf-8", check=False)
+
 
     if error_message and process.returncode != 0:  # 0 means success
         log.error('subprocess error output:')
         if process.stderr:
             log.error(process.stderr)
 
         log.error(error_message)
```

### Comparing `wahoomc-4.0.3a0/wahoomc/resources/sea.osm` & `wahoomc-4.0.3a1/wahoomc/resources/sea.osm`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/resources/shape2osm.py` & `wahoomc-4.0.3a1/wahoomc/resources/shape2osm.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml` & `wahoomc-4.0.3a1/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml` & `wahoomc-4.0.3a1/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml` & `wahoomc-4.0.3a1/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/resources/tags-to-keep.json` & `wahoomc-4.0.3a1/wahoomc/resources/tags-to-keep.json`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/setup_functions.py` & `wahoomc-4.0.3a1/wahoomc/setup_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 
 def check_installation_of_programs_credentials_for_contour_lines():
     """
     check if additionals programs are installed
     """
     text_to_docu = "\nYou have choosen to process contour lines. That needs additional programs. \
-                    \nPlease refer to the Quickstart Guide of wahooMapsCreator for instructions:\n- https://github.com/treee111/wahooMapsCreator/blob/develop/docs/QUICKSTART_ANACONDA.md#additinoal-programs-for-generating-contour-lines \
+                    \nPlease refer to the Quickstart Guide of wahooMapsCreator for instructions:\n- https://github.com/treee111/wahooMapsCreator/blob/develop/docs/QUICKSTART_ANACONDA.md#additional-programs-for-generating-contour-lines \
                     \nor create an issue:\n- https://github.com/treee111/wahooMapsCreator/issues"
 
     if not is_program_installed("phyghtmap"):
         sys.exit(
             f"phyghtmap is not installed. {text_to_docu}")
 
     username, password = read_earthexplorer_credentials()
```

### Comparing `wahoomc-4.0.3a0/wahoomc/tooling_win/7za.dll` & `wahoomc-4.0.3a1/wahoomc/tooling_win/7za.dll`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/tooling_win/7za.exe` & `wahoomc-4.0.3a1/wahoomc/tooling_win/7za.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/tooling_win/7zxa.dll` & `wahoomc-4.0.3a1/wahoomc/tooling_win/7zxa.dll`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/tooling_win/lzma.exe` & `wahoomc-4.0.3a1/wahoomc/tooling_win/lzma.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/tooling_win/osmconvert.exe` & `wahoomc-4.0.3a1/wahoomc/tooling_win/osmconvert.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc/tooling_win/osmconvert64-0.8.8p.exe` & `wahoomc-4.0.3a1/wahoomc/tooling_win/osmconvert64-0.8.8p.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.3a0/wahoomc.egg-info/PKG-INFO` & `wahoomc-4.0.3a1/wahoomc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wahoomc
-Version: 4.0.3a0
+Version: 4.0.3a1
 Summary: Create maps for your Wahoo bike computer based on latest OSM maps
 Home-page: https://github.com/treee111/wahooMapsCreator
 Author: Benjamin Kreuscher
 Author-email: benni.kreuscher@gmail.com
 Project-URL: Bug Tracker, https://github.com/treee111/wahooMapsCreator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wahoomc Version: 4.0.3a0 Summary: Create maps for
+Metadata-Version: 2.1 Name: wahoomc Version: 4.0.3a1 Summary: Create maps for
 your Wahoo bike computer based on latest OSM maps Home-page: https://
 github.com/treee111/wahooMapsCreator Author: Benjamin Kreuscher Author-email:
 benni.kreuscher@gmail.com Project-URL: Bug Tracker, https://github.com/
 treee111/wahooMapsCreator/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.10 Description-Content-Type:
 text/markdown
```

### Comparing `wahoomc-4.0.3a0/wahoomc.egg-info/SOURCES.txt` & `wahoomc-4.0.3a1/wahoomc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

