# Comparing `tmp/eaiscenarioreporter-0.4.6.tar.gz` & `tmp/eaiscenarioreporter-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\eaiscenarioreporter-0.4.6.tar", last modified: Wed Dec 28 21:08:16 2022, max compression
+gzip compressed data, was "dist\eaiscenarioreporter-0.4.7.tar", last modified: Sat Jan 28 15:20:44 2023, max compression
```

## Comparing `eaiscenarioreporter-0.4.6.tar` & `eaiscenarioreporter-0.4.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-12-28 21:08:16.812876 eaiscenarioreporter-0.4.6/
--rw-rw-rw-   0        0        0    35823 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0       82 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6702 2022-12-28 21:08:16.812876 eaiscenarioreporter-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     5933 2022-11-20 15:44:18.000000 eaiscenarioreporter-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2022-12-28 21:08:16.582450 eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/
--rw-rw-rw-   0        0        0     6702 2022-12-28 21:08:15.000000 eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2022-12-28 21:08:15.000000 eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-28 21:08:15.000000 eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2022-12-28 21:08:15.000000 eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2022-12-28 21:08:15.000000 eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-12-28 21:08:15.000000 eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-28 21:08:16.688278 eaiscenarioreporter-0.4.6/featurereporter/
--rw-rw-rw-   0        0        0      147 2022-01-19 08:11:55.000000 eaiscenarioreporter-0.4.6/featurereporter/__init__.py
--rw-rw-rw-   0        0        0      140 2021-09-17 20:11:51.000000 eaiscenarioreporter-0.4.6/featurereporter/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-28 21:08:16.812876 eaiscenarioreporter-0.4.6/featurereporter/assets/
--rw-rw-rw-   0        0        0    17362 2021-04-04 09:10:32.000000 eaiscenarioreporter-0.4.6/featurereporter/assets/COPYING
--rw-rw-rw-   0        0        0    35823 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.6/featurereporter/assets/LICENSE.txt
--rw-rw-rw-   0        0        0  9942607 2022-02-20 20:22:10.000000 eaiscenarioreporter-0.4.6/featurereporter/assets/plantuml.jar
--rw-rw-rw-   0        0        0     3477 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.6/featurereporter/assets/valid.png
--rw-rw-rw-   0        0        0     2852 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.6/featurereporter/assets/warning.png
--rw-rw-rw-   0        0        0    11680 2022-12-28 20:57:51.000000 eaiscenarioreporter-0.4.6/featurereporter/csvformatter.py
--rw-rw-rw-   0        0        0      153 2022-12-23 09:18:31.000000 eaiscenarioreporter-0.4.6/featurereporter/desktopApp.py
--rw-rw-rw-   0        0        0    14908 2022-12-15 20:30:05.000000 eaiscenarioreporter-0.4.6/featurereporter/featurereporter.py
--rw-rw-rw-   0        0        0    27408 2022-12-23 10:14:22.000000 eaiscenarioreporter-0.4.6/featurereporter/reportgenerator.py
--rw-rw-rw-   0        0        0      158 2022-12-28 21:08:16.820558 eaiscenarioreporter-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     2194 2022-12-28 20:57:51.000000 eaiscenarioreporter-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-28 15:20:44.719012 eaiscenarioreporter-0.4.7/
+-rw-rw-rw-   0        0        0    35823 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       82 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6702 2023-01-28 15:20:44.720014 eaiscenarioreporter-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5933 2022-11-20 15:44:18.000000 eaiscenarioreporter-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-01-28 15:20:44.526850 eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/
+-rw-rw-rw-   0        0        0     6702 2023-01-28 15:20:43.000000 eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-01-28 15:20:43.000000 eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-28 15:20:43.000000 eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-01-28 15:20:43.000000 eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       61 2023-01-28 15:20:43.000000 eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-01-28 15:20:43.000000 eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-28 15:20:44.613006 eaiscenarioreporter-0.4.7/featurereporter/
+-rw-rw-rw-   0        0        0      147 2022-01-19 08:11:55.000000 eaiscenarioreporter-0.4.7/featurereporter/__init__.py
+-rw-rw-rw-   0        0        0      140 2021-09-17 20:11:51.000000 eaiscenarioreporter-0.4.7/featurereporter/__main__.py
+drwxrwxrwx   0        0        0        0 2023-01-28 15:20:44.717025 eaiscenarioreporter-0.4.7/featurereporter/assets/
+-rw-rw-rw-   0        0        0    17362 2021-04-04 09:10:32.000000 eaiscenarioreporter-0.4.7/featurereporter/assets/COPYING
+-rw-rw-rw-   0        0        0    35823 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.7/featurereporter/assets/LICENSE.txt
+-rw-rw-rw-   0        0        0  9942607 2022-02-20 20:22:10.000000 eaiscenarioreporter-0.4.7/featurereporter/assets/plantuml.jar
+-rw-rw-rw-   0        0        0     3477 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.7/featurereporter/assets/valid.png
+-rw-rw-rw-   0        0        0     2852 2021-03-13 13:20:04.000000 eaiscenarioreporter-0.4.7/featurereporter/assets/warning.png
+-rw-rw-rw-   0        0        0    11900 2023-01-28 13:55:34.000000 eaiscenarioreporter-0.4.7/featurereporter/csvformatter.py
+-rw-rw-rw-   0        0        0      153 2022-12-23 09:18:31.000000 eaiscenarioreporter-0.4.7/featurereporter/desktopApp.py
+-rw-rw-rw-   0        0        0    14908 2022-12-15 20:30:05.000000 eaiscenarioreporter-0.4.7/featurereporter/featurereporter.py
+-rw-rw-rw-   0        0        0    27408 2022-12-23 10:14:22.000000 eaiscenarioreporter-0.4.7/featurereporter/reportgenerator.py
+-rw-rw-rw-   0        0        0      158 2023-01-28 15:20:44.724013 eaiscenarioreporter-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     2194 2023-01-28 13:56:15.000000 eaiscenarioreporter-0.4.7/setup.py
```

### Comparing `eaiscenarioreporter-0.4.6/LICENSE.txt` & `eaiscenarioreporter-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/PKG-INFO` & `eaiscenarioreporter-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaiscenarioreporter
-Version: 0.4.6
+Version: 0.4.7
 Summary: Turns folder of gherkin feature files into a docx file.
 Home-page: https://github.com/Hidden-goblin/eaiscenarioreporter.git
 Author: Eric Aïvayan
 Author-email: eric.aivayan@free.fr
 Keywords: BDD,Gherkin,behave,docx
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `eaiscenarioreporter-0.4.6/README.md` & `eaiscenarioreporter-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/PKG-INFO` & `eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaiscenarioreporter
-Version: 0.4.6
+Version: 0.4.7
 Summary: Turns folder of gherkin feature files into a docx file.
 Home-page: https://github.com/Hidden-goblin/eaiscenarioreporter.git
 Author: Eric Aïvayan
 Author-email: eric.aivayan@free.fr
 Keywords: BDD,Gherkin,behave,docx
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `eaiscenarioreporter-0.4.6/eaiscenarioreporter.egg-info/SOURCES.txt` & `eaiscenarioreporter-0.4.7/eaiscenarioreporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/featurereporter/assets/COPYING` & `eaiscenarioreporter-0.4.7/featurereporter/assets/COPYING`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/featurereporter/assets/LICENSE.txt` & `eaiscenarioreporter-0.4.7/featurereporter/assets/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/featurereporter/assets/plantuml.jar` & `eaiscenarioreporter-0.4.7/featurereporter/assets/plantuml.jar`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/featurereporter/assets/valid.png` & `eaiscenarioreporter-0.4.7/featurereporter/assets/valid.png`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/featurereporter/assets/warning.png` & `eaiscenarioreporter-0.4.7/featurereporter/assets/warning.png`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/featurereporter/csvformatter.py` & `eaiscenarioreporter-0.4.7/featurereporter/csvformatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- Product under GNU GPL v3 -*-
 # -*- Author: E.Aivayan -*-
 import csv
 import re
 import logging
+from pathlib import Path
 
 from behave.formatter.base import Formatter
 from behave.model import Status
 from csv import DictWriter
 
 log = logging.getLogger(__name__)
 
@@ -131,14 +132,15 @@
         self.__current_epic = None
         self.__current_scenario_name = None
         self.__current_scenario_id = None
         self.__current_status = None
         self.__outline_order = None
         self.__current_feature_model = None
         self.__current_scenario_model = None
+        self.__base_dir = str(Path(config.base_dir).resolve().absolute())
         # UserData
         if "userdata" in config.defaults and "EaiCsv.epic" in config.defaults["userdata"]:
             self.__epic = config.defaults["userdata"]["EaiCsv.epic"]
         else:
             self.__epic = "epic="
 
         if "userdata" in config.defaults and "EaiCsv.scenario" in config.defaults["userdata"]:
@@ -151,16 +153,18 @@
     def feature(self, feature):
         self.__current_feature = feature.name
         for tag in feature.tags:
             self.__current_epic = None
             if self.__epic in tag:
                 self.__current_epic = tag.replace(self.__epic, "")
                 break
+        filename = str(Path(feature.filename).resolve().absolute())
+        filename = filename.replace(self.__base_dir, "")
         self.__current_feature_model = FeatureModel(feature.name,
-                                                    feature.filename,
+                                                    filename,
                                                     self.__current_epic,
                                                     feature.tags,
                                                     feature.description)
         self.__epics.add(self.__current_epic)
         self.__features.append(self.__current_feature_model.to_dict())
 
     def scenario(self, scenario):
```

### Comparing `eaiscenarioreporter-0.4.6/featurereporter/featurereporter.py` & `eaiscenarioreporter-0.4.7/featurereporter/featurereporter.py`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/featurereporter/reportgenerator.py` & `eaiscenarioreporter-0.4.7/featurereporter/reportgenerator.py`

 * *Files identical despite different names*

### Comparing `eaiscenarioreporter-0.4.6/setup.py` & `eaiscenarioreporter-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="eaiscenarioreporter",
-    version="0.4.6",
+    version="0.4.7",
     description="Turns folder of gherkin feature files into a docx file.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
```

