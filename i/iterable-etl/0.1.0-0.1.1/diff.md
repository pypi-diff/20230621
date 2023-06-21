# Comparing `tmp/iterable_etl-0.1.0.tar.gz` & `tmp/iterable_etl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable_etl-0.1.0.tar", last modified: Wed Jun 14 17:47:55 2023, max compression
+gzip compressed data, was "iterable_etl-0.1.1.tar", last modified: Wed Jun 21 18:40:23 2023, max compression
```

## Comparing `iterable_etl-0.1.0.tar` & `iterable_etl-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:47:55.877673 iterable_etl-0.1.0/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.1.0/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2027 2023-06-14 17:47:55.877673 iterable_etl-0.1.0/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1519 2023-06-14 17:30:32.000000 iterable_etl-0.1.0/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:47:55.873673 iterable_etl-0.1.0/iterable_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 17:47:33.000000 iterable_etl-0.1.0/iterable_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      155 2023-06-14 17:33:42.000000 iterable_etl-0.1.0/iterable_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      834 2023-06-14 17:33:42.000000 iterable_etl-0.1.0/iterable_etl/iterable_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:47:55.873673 iterable_etl-0.1.0/iterable_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.1.0/iterable_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      589 2023-06-14 17:41:44.000000 iterable_etl-0.1.0/iterable_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-14 17:33:42.000000 iterable_etl-0.1.0/iterable_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1086 2023-06-14 17:42:26.000000 iterable_etl-0.1.0/iterable_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      636 2023-06-07 19:11:13.000000 iterable_etl-0.1.0/iterable_etl/libs/spark.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      928 2023-06-14 17:33:42.000000 iterable_etl-0.1.0/iterable_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:47:55.873673 iterable_etl-0.1.0/iterable_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.1.0/iterable_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      843 2023-06-14 17:39:05.000000 iterable_etl-0.1.0/iterable_etl/tables/campaign_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1370 2023-06-14 17:39:18.000000 iterable_etl-0.1.0/iterable_etl/tables/campaign_list_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1723 2023-06-14 17:39:50.000000 iterable_etl-0.1.0/iterable_etl/tables/campaign_metrics.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      769 2023-06-14 17:40:00.000000 iterable_etl-0.1.0/iterable_etl/tables/list.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:47:55.873673 iterable_etl-0.1.0/iterable_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2027 2023-06-14 17:47:55.000000 iterable_etl-0.1.0/iterable_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      676 2023-06-14 17:47:55.000000 iterable_etl-0.1.0/iterable_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 17:47:55.000000 iterable_etl-0.1.0/iterable_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-14 17:47:55.000000 iterable_etl-0.1.0/iterable_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-14 17:47:55.000000 iterable_etl-0.1.0/iterable_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      426 2023-06-14 17:47:55.877673 iterable_etl-0.1.0/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1050 2023-06-14 17:47:33.000000 iterable_etl-0.1.0/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:47:55.877673 iterable_etl-0.1.0/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.1.0/tests/__init__.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      307 2023-06-09 16:43:58.000000 iterable_etl-0.1.1/MANIFEST.in
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1519 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/README_PUBLIC.md
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.058696 iterable_etl-0.1.1/iterable_etl/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       22 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      155 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/__main__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1006 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/iterable_etl.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/iterable_etl/libs/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.1/iterable_etl/libs/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      667 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/libs/cnst.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1629 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/libs/dbg.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1086 2023-06-21 17:16:40.000000 iterable_etl-0.1.1/iterable_etl/libs/network.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1403 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/libs/spark.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      928 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/libs/transform.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/iterable_etl/tables/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.1/iterable_etl/tables/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      843 2023-06-21 17:33:07.000000 iterable_etl-0.1.1/iterable_etl/tables/campaign_history.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1370 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/tables/campaign_list_history.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1723 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/tables/campaign_metrics.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      769 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/tables/list.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1937 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/tables/list_user_history.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/iterable_etl.egg-info/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      717 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       75 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/requires.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       13 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/top_level.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      426 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/setup.cfg
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1050 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/setup.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/tests/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.1/tests/__init__.py
```

### Comparing `iterable_etl-0.1.0/PKG-INFO` & `iterable_etl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable_etl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.1.0/README_PUBLIC.md` & `iterable_etl-0.1.1/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.0/iterable_etl/iterable_etl.py` & `iterable_etl-0.1.1/iterable_etl/iterable_etl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """cli"""
 import click
 
 from iterable_etl.tables.campaign_history import campaign_history_df
 from iterable_etl.tables.campaign_list_history import campaign_list_history_df
 from iterable_etl.tables.campaign_metrics import campaign_metrics_df
 from iterable_etl.tables.list import list_df
+from iterable_etl.tables.list_user_history import list_user_history_df
 
 
 @click.command()
 @click.option("--table")
 def main(table: str) -> None:
     """program"""
     if table == "campaign_history":
         campaign_history_df()
     elif table == "campaign_metrics":
         campaign_metrics_df()
     elif table == "list":
         list_df()
     elif table == "campaign_list_history":
         campaign_list_history_df()
+    elif table == "list_user_history":
+        list_user_history_df()
     elif table == "ALL":
         campaign_history_df()
         campaign_metrics_df()
         list_df()
         campaign_list_history_df()
+        list_user_history_df()
     else:
         raise ValueError("Invalid table selection")
```

### Comparing `iterable_etl-0.1.0/iterable_etl/libs/cnst.py` & `iterable_etl-0.1.1/iterable_etl/libs/cnst.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """constants"""
 
 import os
 from datetime import date
-from typing import Dict, Any
+from typing import Any, Dict
 
 urls = {
     "lists": "https://api.iterable.com/api/lists",
     "campaigns": "https://api.iterable.com/api/campaigns",
     "metrics": "https://api.iterable.com/api/campaigns/metrics",
+    "lists_get_users": "https://api.iterable.com/api/lists/getUsers?listId=",
 }
 
 
 def get_headers() -> Dict[str, Any]:
     """header config for Iterable API"""
     headers = {
         "Api-Key": os.environ.get("ITERABLE_KEY"),
```

### Comparing `iterable_etl-0.1.0/iterable_etl/libs/dbg.py` & `iterable_etl-0.1.1/iterable_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.0/iterable_etl/libs/network.py` & `iterable_etl-0.1.1/iterable_etl/libs/network.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.0/iterable_etl/libs/transform.py` & `iterable_etl-0.1.1/iterable_etl/libs/transform.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.0/iterable_etl/tables/campaign_history.py` & `iterable_etl-0.1.1/iterable_etl/tables/campaign_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.0/iterable_etl/tables/campaign_list_history.py` & `iterable_etl-0.1.1/iterable_etl/tables/campaign_list_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.0/iterable_etl/tables/campaign_metrics.py` & `iterable_etl-0.1.1/iterable_etl/tables/campaign_metrics.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.0/iterable_etl/tables/list.py` & `iterable_etl-0.1.1/iterable_etl/tables/list.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.0/iterable_etl.egg-info/PKG-INFO` & `iterable_etl-0.1.1/iterable_etl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable-etl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.1.0/iterable_etl.egg-info/SOURCES.txt` & `iterable_etl-0.1.1/iterable_etl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 iterable_etl/libs/spark.py
 iterable_etl/libs/transform.py
 iterable_etl/tables/__init__.py
 iterable_etl/tables/campaign_history.py
 iterable_etl/tables/campaign_list_history.py
 iterable_etl/tables/campaign_metrics.py
 iterable_etl/tables/list.py
+iterable_etl/tables/list_user_history.py
 tests/__init__.py
```

### Comparing `iterable_etl-0.1.0/setup.py` & `iterable_etl-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="iterable_etl",
-    version="0.1.0",
+    version="0.1.1",
     description="Replicate iterable data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

