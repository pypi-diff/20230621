# Comparing `tmp/nowcasting_datamodel-1.4.3.tar.gz` & `tmp/nowcasting_datamodel-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.4.3.tar", last modified: Wed Jun 21 13:49:00 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.4.4.tar", last modified: Wed Jun 21 14:04:59 2023, max compression
```

## Comparing `nowcasting_datamodel-1.4.3.tar` & `nowcasting_datamodel-1.4.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.275698 nowcasting_datamodel-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-21 13:49:00.275698 nowcasting_datamodel-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.271698 nowcasting_datamodel-1.4.3/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.271698 nowcasting_datamodel-1.4.3/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.271698 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.275698 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.275698 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.275698 nowcasting_datamodel-1.4.3/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.271698 nowcasting_datamodel-1.4.3/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-21 13:49:00.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-21 13:49:00.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:49:00.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 13:49:00.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 13:49:00.000000 nowcasting_datamodel-1.4.3/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:49:00.275698 nowcasting_datamodel-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:49:00.275698 nowcasting_datamodel-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-21 13:48:48.000000 nowcasting_datamodel-1.4.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.194617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.194617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.194617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.194617 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.4.3/PKG-INFO` & `nowcasting_datamodel-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.4.3
+Version: 1.4.4
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.3/README.md` & `nowcasting_datamodel-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/diagram.png` & `nowcasting_datamodel-1.4.4/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/diagram_pv.png` & `nowcasting_datamodel-1.4.4/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/api.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/api.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_pv.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,29 +148,35 @@
 def get_pv_yield(
     session: Session,
     pv_systems_ids: Optional[List[int]] = None,
     start_utc: Optional[datetime] = None,
     end_utc: Optional[datetime] = None,
     correct_data: Optional[bool] = None,
     providers: Optional[List[str]] = None,
+    distinct: Optional[bool] = False,
 ) -> Union[List[PVYieldSQL], List[PVSystemSQL]]:
     """
     Get the last pv yield data
 
     :param session: database sessions
     :param pv_systems_ids: list of pv systems ids
     :param end_utc: search filters < on 'datetime_utc'. Can be None
     :param start_utc: search filters >= on 'datetime_utc'. Can be None
     :param correct_data: Filters on incorrect_data in pv_systems
     :param providers: optional list of provider names
+    :param distinct: if True, only return distinct pv yields
     :return: either list of pv yields, or pv systems
     """
 
     # start main query
     query = session.query(PVYieldSQL)
+
+    if distinct:
+        query = query.distinct(PVSystemSQL.id, PVYieldSQL.datetime_utc)
+
     query = query.join(PVSystemSQL)
     query = query.options(joinedload(PVYieldSQL.pv_system))
 
     # only select correct data pv systems
     if correct_data is not None:
         query = query.filter(PVSystemSQL.correct_data == correct_data)
 
@@ -189,14 +195,15 @@
     if providers is not None:
         query = query.filter(PVSystemSQL.provider.in_(providers))
 
     # order by 'created_utc' desc, so we get the latest one
     query = query.order_by(
         PVSystemSQL.id,
         PVYieldSQL.datetime_utc,
+        PVYieldSQL.created_utc.desc(),
     )
 
     # get all results
     pv_yields: List[PVYieldSQL] = query.all()
 
     for pv_yield in pv_yields:
         pv_yield.datetime_utc = pv_yield.datetime_utc.replace(tzinfo=timezone.utc)
```

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/read/read_user.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_user.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.4.3
+Version: 1.4.4
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.3/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/setup.py` & `nowcasting_datamodel-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.4.4/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/tests/test_fake.py` & `nowcasting_datamodel-1.4.4/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/tests/test_fake_pv.py` & `nowcasting_datamodel-1.4.4/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/tests/test_national.py` & `nowcasting_datamodel-1.4.4/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.3/tests/test_utils.py` & `nowcasting_datamodel-1.4.4/tests/test_utils.py`

 * *Files identical despite different names*

