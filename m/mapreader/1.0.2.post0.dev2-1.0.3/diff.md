# Comparing `tmp/mapreader-1.0.2.post0.dev2.tar.gz` & `tmp/mapreader-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapreader-1.0.2.post0.dev2.tar", last modified: Wed Jun 21 07:32:52 2023, max compression
+gzip compressed data, was "mapreader-1.0.3.tar", last modified: Wed Jun 21 14:25:47 2023, max compression
```

## Comparing `mapreader-1.0.2.post0.dev2.tar` & `mapreader-1.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.845488 mapreader-1.0.2.post0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-21 07:32:52.845488 mapreader-1.0.2.post0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.849488 mapreader-1.0.2.post0.dev2/mapreader/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-21 07:32:52.849488 mapreader-1.0.2.post0.dev2/mapreader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.841488 mapreader-1.0.2.post0.dev2/mapreader/annotate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/annotate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.841488 mapreader-1.0.2.post0.dev2/mapreader/classify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73307 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/classify/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    27268 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/classify/classifier_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/classify/custom_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28572 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/classify/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/classify/load_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.845488 mapreader-1.0.2.post0.dev2/mapreader/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/download/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/download/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38174 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/download/sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/download/tile_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/download/tile_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.845488 mapreader-1.0.2.post0.dev2/mapreader/load/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/load/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86859 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/load/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/load/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.845488 mapreader-1.0.2.post0.dev2/mapreader/process/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/process/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.845488 mapreader-1.0.2.post0.dev2/mapreader/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/utils/compute_and_save_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/mapreader/utils/slice_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.841488 mapreader-1.0.2.post0.dev2/mapreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-21 07:32:52.000000 mapreader-1.0.2.post0.dev2/mapreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-21 07:32:52.000000 mapreader-1.0.2.post0.dev2/mapreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:32:52.000000 mapreader-1.0.2.post0.dev2/mapreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 07:32:52.000000 mapreader-1.0.2.post0.dev2/mapreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:32:52.000000 mapreader-1.0.2.post0.dev2/mapreader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 07:32:52.000000 mapreader-1.0.2.post0.dev2/mapreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 07:32:52.000000 mapreader-1.0.2.post0.dev2/mapreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 07:32:52.845488 mapreader-1.0.2.post0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:32:52.845488 mapreader-1.0.2.post0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/tests/test_annotations_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/tests/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/tests/test_sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-21 07:32:37.000000 mapreader-1.0.2.post0.dev2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-21 14:25:35.000000 mapreader-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-21 14:25:47.145010 mapreader-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-21 14:25:35.000000 mapreader-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/mapreader/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 14:25:47.145010 mapreader-1.0.3/mapreader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.137010 mapreader-1.0.3/mapreader/annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/annotate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.141010 mapreader-1.0.3/mapreader/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73307 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27268 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/classifier_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/custom_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28572 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/classify/load_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.141010 mapreader-1.0.3/mapreader/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38174 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/tile_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/download/tile_merging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.141010 mapreader-1.0.3/mapreader/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/load/geo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86859 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/load/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/load/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/mapreader/process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/process/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/mapreader/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/utils/compute_and_save_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 14:25:35.000000 mapreader-1.0.3/mapreader/utils/slice_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.137010 mapreader-1.0.3/mapreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:25:46.000000 mapreader-1.0.3/mapreader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 14:25:47.000000 mapreader-1.0.3/mapreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 14:25:47.145010 mapreader-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-21 14:25:35.000000 mapreader-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:47.145010 mapreader-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-21 14:25:35.000000 mapreader-1.0.3/tests/test_annotations_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-21 14:25:35.000000 mapreader-1.0.3/tests/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-21 14:25:35.000000 mapreader-1.0.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-06-21 14:25:35.000000 mapreader-1.0.3/tests/test_sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-21 14:25:35.000000 mapreader-1.0.3/versioneer.py
```

### Comparing `mapreader-1.0.2.post0.dev2/LICENSE` & `mapreader-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/PKG-INFO` & `mapreader-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.0.2.post0.dev2
+Version: 1.0.3
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.0.2.post0.dev2 Summary: A
-computer vision pipeline for the semantic exploration of maps/images at scale
-Home-page: https://github.com/Living-with-machines/MapReader Download-URL:
-https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
-Author: MapReader team License: MIT License Keywords: Computer
-Vision,Classification,Deep Learning,living with machines Platform: OS
-Independent Classifier: Development Status :: 3 - Alpha Classifier: License ::
-OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Intended Audience :: End Users/Desktop Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research Classifier: Operating System
-:: Unix Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7, <3.11
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: mapreader Version: 1.0.3 Summary: A computer vision
+pipeline for the semantic exploration of maps/images at scale Home-page: https:
+//github.com/Living-with-machines/MapReader Download-URL: https://github.com/
+Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
+team License: MIT License Keywords: Computer Vision,Classification,Deep
+Learning,living with machines Platform: OS Independent Classifier: Development
+Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Education Classifier: Intended
+Audience :: Science/Research Classifier: Operating System :: Unix Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
+Classifier: Operating System :: OS Independent Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7, <3.11 Description-Content-Type: text/markdown License-
+File: LICENSE
 
                             ****** MapReader ******
  ***** A computer vision pipeline for exploring and analyzing images at scale
                                      *****
                   [PyPI] [License] [Integration_Tests_badge]
 ## What is MapReader?
                     [Annotated Map with Prediction Outputs]
```

### Comparing `mapreader-1.0.2.post0.dev2/README.md` & `mapreader-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/__init__.py` & `mapreader-1.0.3/mapreader/__init__.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/annotate/utils.py` & `mapreader-1.0.3/mapreader/annotate/utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/classify/classifier.py` & `mapreader-1.0.3/mapreader/classify/classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/classify/classifier_context.py` & `mapreader-1.0.3/mapreader/classify/classifier_context.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/classify/custom_models.py` & `mapreader-1.0.3/mapreader/classify/custom_models.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/classify/datasets.py` & `mapreader-1.0.3/mapreader/classify/datasets.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/classify/load_annotations.py` & `mapreader-1.0.3/mapreader/classify/load_annotations.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/download/data_structures.py` & `mapreader-1.0.3/mapreader/download/data_structures.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/download/downloader.py` & `mapreader-1.0.3/mapreader/download/downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/download/downloader_utils.py` & `mapreader-1.0.3/mapreader/download/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/download/sheet_downloader.py` & `mapreader-1.0.3/mapreader/download/sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/download/tile_loading.py` & `mapreader-1.0.3/mapreader/download/tile_loading.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/download/tile_merging.py` & `mapreader-1.0.3/mapreader/download/tile_merging.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/load/geo_utils.py` & `mapreader-1.0.3/mapreader/load/geo_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/load/images.py` & `mapreader-1.0.3/mapreader/load/images.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/load/loader.py` & `mapreader-1.0.3/mapreader/load/loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/process/process.py` & `mapreader-1.0.3/mapreader/process/process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/utils/compute_and_save_stats.py` & `mapreader-1.0.3/mapreader/utils/compute_and_save_stats.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader/utils/slice_parallel.py` & `mapreader-1.0.3/mapreader/utils/slice_parallel.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader.egg-info/PKG-INFO` & `mapreader-1.0.3/mapreader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.0.2.post0.dev2
+Version: 1.0.3
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.0.2.post0.dev2 Summary: A
-computer vision pipeline for the semantic exploration of maps/images at scale
-Home-page: https://github.com/Living-with-machines/MapReader Download-URL:
-https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
-Author: MapReader team License: MIT License Keywords: Computer
-Vision,Classification,Deep Learning,living with machines Platform: OS
-Independent Classifier: Development Status :: 3 - Alpha Classifier: License ::
-OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Intended Audience :: End Users/Desktop Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research Classifier: Operating System
-:: Unix Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7, <3.11
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: mapreader Version: 1.0.3 Summary: A computer vision
+pipeline for the semantic exploration of maps/images at scale Home-page: https:
+//github.com/Living-with-machines/MapReader Download-URL: https://github.com/
+Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
+team License: MIT License Keywords: Computer Vision,Classification,Deep
+Learning,living with machines Platform: OS Independent Classifier: Development
+Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Education Classifier: Intended
+Audience :: Science/Research Classifier: Operating System :: Unix Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
+Classifier: Operating System :: OS Independent Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7, <3.11 Description-Content-Type: text/markdown License-
+File: LICENSE
 
                             ****** MapReader ******
  ***** A computer vision pipeline for exploring and analyzing images at scale
                                      *****
                   [PyPI] [License] [Integration_Tests_badge]
 ## What is MapReader?
                     [Annotated Map with Prediction Outputs]
```

### Comparing `mapreader-1.0.2.post0.dev2/mapreader.egg-info/SOURCES.txt` & `mapreader-1.0.3/mapreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/mapreader.egg-info/requires.txt` & `mapreader-1.0.3/mapreader.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/setup.py` & `mapreader-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/tests/test_annotations_loader.py` & `mapreader-1.0.3/tests/test_annotations_loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/tests/test_classifier.py` & `mapreader-1.0.3/tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/tests/test_import.py` & `mapreader-1.0.3/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/tests/test_sheet_downloader.py` & `mapreader-1.0.3/tests/test_sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.2.post0.dev2/versioneer.py` & `mapreader-1.0.3/versioneer.py`

 * *Files identical despite different names*

