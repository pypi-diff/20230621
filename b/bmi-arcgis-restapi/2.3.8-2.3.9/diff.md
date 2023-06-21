# Comparing `tmp/bmi-arcgis-restapi-2.3.8.tar.gz` & `tmp/bmi-arcgis-restapi-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmi-arcgis-restapi-2.3.8.tar", last modified: Mon May 15 14:16:01 2023, max compression
+gzip compressed data, was "bmi-arcgis-restapi-2.3.9.tar", last modified: Fri May 26 19:53:51 2023, max compression
```

## Comparing `bmi-arcgis-restapi-2.3.8.tar` & `bmi-arcgis-restapi-2.3.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.306888 bmi-arcgis-restapi-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43529 2023-05-15 14:16:01.306888 bmi-arcgis-restapi-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43756 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.294888 bmi-arcgis-restapi-2.3.8/bmi_arcgis_restapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43529 2023-05-15 14:16:01.000000 bmi-arcgis-restapi-2.3.8/bmi_arcgis_restapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-15 14:16:01.000000 bmi-arcgis-restapi-2.3.8/bmi_arcgis_restapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:16:01.000000 bmi-arcgis-restapi-2.3.8/bmi_arcgis_restapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 14:16:01.000000 bmi-arcgis-restapi-2.3.8/bmi_arcgis_restapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 14:16:01.000000 bmi-arcgis-restapi-2.3.8/bmi_arcgis_restapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.294888 bmi-arcgis-restapi-2.3.8/restapi/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/_strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.294888 bmi-arcgis-restapi-2.3.8/restapi/admin/
--rw-r--r--   0 runner    (1001) docker     (123)   129756 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.294888 bmi-arcgis-restapi-2.3.8/restapi/admin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/admin/samples/admin_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/admin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28063 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/arc_restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)   166239 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.294888 bmi-arcgis-restapi-2.3.8/restapi/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)    16306 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.298888 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.298888 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/css/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/css/app.615af0e5.css
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/css/chunk-26ed89da.8fb689c1.css
--rw-r--r--   0 runner    (1001) docker     (123)   219149 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/css/chunk-vendors.64d43e69.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.294888 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.298888 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    29808 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/android-chrome-maskable-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/android-chrome-maskable-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/msapplication-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.298888 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/js/app.dbaf9f92.js
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/js/chunk-26ed89da.db4a4cda.js
--rw-r--r--   0 runner    (1001) docker     (123)   347124 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/js/chunk-vendors.20697101.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/precache-manifest.b62ded22fc8a9700861c815d7e20acbd.js
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/service-worker.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20762 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/open_restapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.298888 bmi-arcgis-restapi-2.3.8/restapi/projections/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/projections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.302888 bmi-arcgis-restapi-2.3.8/restapi/projections/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   964212 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/projections/bin/gtf.json
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/projections/bin/linearUnits.json
--rw-r--r--   0 runner    (1001) docker     (123)   188627 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/projections/bin/projection_names.json
--rw-r--r--   0 runner    (1001) docker     (123)  2060997 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/projections/bin/projection_strings.json
--rw-r--r--   0 runner    (1001) docker     (123)  2269080 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/projections/bin/projections.json
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/rest_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    75045 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/shapefile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:16:01.306888 bmi-arcgis-restapi-2.3.8/restapi/shp_helper/
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/restapi/shp_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 14:16:01.306888 bmi-arcgis-restapi-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-15 14:15:51.000000 bmi-arcgis-restapi-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.290593 bmi-arcgis-restapi-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43681 2023-05-26 19:53:51.290593 bmi-arcgis-restapi-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43756 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.270593 bmi-arcgis-restapi-2.3.9/bmi_arcgis_restapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43681 2023-05-26 19:53:51.000000 bmi-arcgis-restapi-2.3.9/bmi_arcgis_restapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-26 19:53:51.000000 bmi-arcgis-restapi-2.3.9/bmi_arcgis_restapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:53:51.000000 bmi-arcgis-restapi-2.3.9/bmi_arcgis_restapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 19:53:51.000000 bmi-arcgis-restapi-2.3.9/bmi_arcgis_restapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 19:53:51.000000 bmi-arcgis-restapi-2.3.9/bmi_arcgis_restapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.270593 bmi-arcgis-restapi-2.3.9/restapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.270593 bmi-arcgis-restapi-2.3.9/restapi/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)   129756 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.274593 bmi-arcgis-restapi-2.3.9/restapi/admin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/admin/samples/admin_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/admin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28063 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/arc_restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166239 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.274593 bmi-arcgis-restapi-2.3.9/restapi/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)    16306 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.274593 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.274593 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/css/app.615af0e5.css
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/css/chunk-26ed89da.8fb689c1.css
+-rw-r--r--   0 runner    (1001) docker     (123)   219149 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/css/chunk-vendors.64d43e69.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.266593 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.278593 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29808 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/android-chrome-maskable-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/android-chrome-maskable-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/msapplication-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.278593 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/js/app.dbaf9f92.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/js/chunk-26ed89da.db4a4cda.js
+-rw-r--r--   0 runner    (1001) docker     (123)   347124 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/js/chunk-vendors.20697101.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/precache-manifest.b62ded22fc8a9700861c815d7e20acbd.js
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/service-worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20762 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/open_restapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.278593 bmi-arcgis-restapi-2.3.9/restapi/projections/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/projections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.286593 bmi-arcgis-restapi-2.3.9/restapi/projections/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   964212 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/projections/bin/gtf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/projections/bin/linearUnits.json
+-rw-r--r--   0 runner    (1001) docker     (123)   188627 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/projections/bin/projection_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2060997 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/projections/bin/projection_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2269080 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/projections/bin/projections.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/rest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75045 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/shapefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:53:51.290593 bmi-arcgis-restapi-2.3.9/restapi/shp_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/restapi/shp_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 19:53:51.290593 bmi-arcgis-restapi-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-26 19:53:33.000000 bmi-arcgis-restapi-2.3.9/setup.py
```

### Comparing `bmi-arcgis-restapi-2.3.8/LICENSE` & `bmi-arcgis-restapi-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/PKG-INFO` & `bmi-arcgis-restapi-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmi-arcgis-restapi
-Version: 2.3.8
+Version: 2.3.9
 Summary: Package for working with ArcGIS REST API
 Home-page: https://github.com/Bolton-and-Menk-GIS/restapi
 Author: Caleb Mackey
 Author-email: calebma@bolton-menk.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,17 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # restapi
 
 This is a Python API for working with ArcGIS REST API, ArcGIS Online, and Portal/ArcGIS Enterprise.  This package has been designed to work with [arcpy](https://pro.arcgis.com/en/pro-app/arcpy/get-started/what-is-arcpy-.htm) when available, or the included open source module [pyshp](https://pypi.org/project/pyshp/).  It will try to use arcpy if available for some data conversions, otherwise will use open source options. Also included is a subpackage for administering ArcGIS Server Sites.  This is updated often, so continue checking here for new functionality!
```

### Comparing `bmi-arcgis-restapi-2.3.8/README.md` & `bmi-arcgis-restapi-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/bmi_arcgis_restapi.egg-info/PKG-INFO` & `bmi-arcgis-restapi-2.3.9/bmi_arcgis_restapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmi-arcgis-restapi
-Version: 2.3.8
+Version: 2.3.9
 Summary: Package for working with ArcGIS REST API
 Home-page: https://github.com/Bolton-and-Menk-GIS/restapi
 Author: Caleb Mackey
 Author-email: calebma@bolton-menk.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,17 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # restapi
 
 This is a Python API for working with ArcGIS REST API, ArcGIS Online, and Portal/ArcGIS Enterprise.  This package has been designed to work with [arcpy](https://pro.arcgis.com/en/pro-app/arcpy/get-started/what-is-arcpy-.htm) when available, or the included open source module [pyshp](https://pypi.org/project/pyshp/).  It will try to use arcpy if available for some data conversions, otherwise will use open source options. Also included is a subpackage for administering ArcGIS Server Sites.  This is updated often, so continue checking here for new functionality!
```

### Comparing `bmi-arcgis-restapi-2.3.8/bmi_arcgis_restapi.egg-info/SOURCES.txt` & `bmi-arcgis-restapi-2.3.9/bmi_arcgis_restapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/__init__.py` & `bmi-arcgis-restapi-2.3.9/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/_strings.py` & `bmi-arcgis-restapi-2.3.9/restapi/_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
 
 FIELD_KEYS_CREATE = [NAME, ALIAS, TYPE, DOMAIN, LENGTH]
 
 GEOM_CODE = {v:k for k,v in six.iteritems(GEOM_DICT)}
 BASE_PATTERN = 'http*://*/rest/services*'
 PORTAL_BASE_PATTERN = 'http*://*/sharing/rest*'
 PORTAL_SERVICES_PATTERN = 'http*://*/sharing/servers/*/rest/services/*'
-VERSION = '2.3.8'
+VERSION = '2.3.9'
 PACKAGE_NAME = 'restapi'
 USER_AGENT = '{}/{} (Python)'.format(PACKAGE_NAME, VERSION)
 GET = 'GET'
 POST = 'POST'
 
 PROTOCOL = ''
```

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/admin/__init__.py` & `bmi-arcgis-restapi-2.3.9/restapi/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/admin/samples/admin_samples.py` & `bmi-arcgis-restapi-2.3.9/restapi/admin/samples/admin_samples.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/admin/utils.py` & `bmi-arcgis-restapi-2.3.9/restapi/admin/utils.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/arc_restapi.py` & `bmi-arcgis-restapi-2.3.9/restapi/arc_restapi.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/common_types.py` & `bmi-arcgis-restapi-2.3.9/restapi/common_types.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/conversion.py` & `bmi-arcgis-restapi-2.3.9/restapi/conversion.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/decorator/__init__.py` & `bmi-arcgis-restapi-2.3.9/restapi/decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/enums.py` & `bmi-arcgis-restapi-2.3.9/restapi/enums.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/exceptions.py` & `bmi-arcgis-restapi-2.3.9/restapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/css/chunk-26ed89da.8fb689c1.css` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/css/chunk-26ed89da.8fb689c1.css`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/css/chunk-vendors.64d43e69.css` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/css/chunk-vendors.64d43e69.css`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/favicon.ico` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/favicon.ico`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/android-chrome-192x192.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/android-chrome-512x512.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/android-chrome-maskable-192x192.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/android-chrome-maskable-192x192.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/android-chrome-maskable-512x512.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/android-chrome-maskable-512x512.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-120x120.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-152x152.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-180x180.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-60x60.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon-76x76.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/apple-touch-icon.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/favicon-16x16.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/favicon-32x32.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/msapplication-icon-144x144.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/msapplication-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/img/icons/mstile-150x150.png` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/img/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/index.html` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/index.html`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/js/app.dbaf9f92.js` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/js/app.dbaf9f92.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/js/chunk-26ed89da.db4a4cda.js` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/js/chunk-26ed89da.db4a4cda.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/js/chunk-vendors.20697101.js` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/js/chunk-vendors.20697101.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/manifest.json` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/manifest.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/precache-manifest.b62ded22fc8a9700861c815d7e20acbd.js` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/precache-manifest.b62ded22fc8a9700861c815d7e20acbd.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/geometry-helper/service-worker.js` & `bmi-arcgis-restapi-2.3.9/restapi/geometry-helper/service-worker.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/globals.py` & `bmi-arcgis-restapi-2.3.9/restapi/globals.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/open_restapi.py` & `bmi-arcgis-restapi-2.3.9/restapi/open_restapi.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/projections/__init__.py` & `bmi-arcgis-restapi-2.3.9/restapi/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/projections/bin/gtf.json` & `bmi-arcgis-restapi-2.3.9/restapi/projections/bin/gtf.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/projections/bin/linearUnits.json` & `bmi-arcgis-restapi-2.3.9/restapi/projections/bin/linearUnits.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/projections/bin/projection_names.json` & `bmi-arcgis-restapi-2.3.9/restapi/projections/bin/projection_names.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/projections/bin/projection_strings.json` & `bmi-arcgis-restapi-2.3.9/restapi/projections/bin/projection_strings.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/projections/bin/projections.json` & `bmi-arcgis-restapi-2.3.9/restapi/projections/bin/projections.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/rest_utils.py` & `bmi-arcgis-restapi-2.3.9/restapi/rest_utils.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/shapefile.py` & `bmi-arcgis-restapi-2.3.9/restapi/shapefile.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/restapi/shp_helper/__init__.py` & `bmi-arcgis-restapi-2.3.9/restapi/shp_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.8/setup.py` & `bmi-arcgis-restapi-2.3.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 name = 'bmi-arcgis-restapi'
 
 setup(name=name,
-      version='2.3.8',
+      version='2.3.9',
       description='Package for working with ArcGIS REST API',
       author='Caleb Mackey',
       author_email='calebma@bolton-menk.com',
       url='https://github.com/Bolton-and-Menk-GIS/restapi',
       license='GPL',
       packages=find_packages(),
       include_package_data=True,
@@ -33,10 +33,13 @@
           'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.4',
           'Programming Language :: Python :: 3.5',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Topic :: Scientific/Engineering :: GIS'
       ]
 )
```

