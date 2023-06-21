# Comparing `tmp/iterable_etl-0.1.1.tar.gz` & `tmp/iterable_etl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable_etl-0.1.1.tar", last modified: Wed Jun 21 18:40:23 2023, max compression
+gzip compressed data, was "iterable_etl-0.1.2.tar", last modified: Wed Jun 21 19:34:48 2023, max compression
```

## Comparing `iterable_etl-0.1.1.tar` & `iterable_etl-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      307 2023-06-09 16:43:58.000000 iterable_etl-0.1.1/MANIFEST.in
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1519 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/README_PUBLIC.md
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.058696 iterable_etl-0.1.1/iterable_etl/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       22 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      155 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/__main__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1006 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/iterable_etl.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/iterable_etl/libs/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.1/iterable_etl/libs/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      667 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/libs/cnst.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1629 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/libs/dbg.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1086 2023-06-21 17:16:40.000000 iterable_etl-0.1.1/iterable_etl/libs/network.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1403 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/libs/spark.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      928 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/libs/transform.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/iterable_etl/tables/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.1/iterable_etl/tables/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      843 2023-06-21 17:33:07.000000 iterable_etl-0.1.1/iterable_etl/tables/campaign_history.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1370 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/tables/campaign_list_history.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1723 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/tables/campaign_metrics.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      769 2023-06-21 16:51:38.000000 iterable_etl-0.1.1/iterable_etl/tables/list.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1937 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/iterable_etl/tables/list_user_history.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/iterable_etl.egg-info/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      717 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       75 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/requires.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       13 2023-06-21 18:40:22.000000 iterable_etl-0.1.1/iterable_etl.egg-info/top_level.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      426 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/setup.cfg
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1050 2023-06-21 18:38:35.000000 iterable_etl-0.1.1/setup.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 18:40:23.062696 iterable_etl-0.1.1/tests/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.1/tests/__init__.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 19:34:48.560997 iterable_etl-0.1.2/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      307 2023-06-09 16:43:58.000000 iterable_etl-0.1.2/MANIFEST.in
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-21 19:34:48.560997 iterable_etl-0.1.2/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1519 2023-06-21 16:51:38.000000 iterable_etl-0.1.2/README_PUBLIC.md
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 19:34:48.556997 iterable_etl-0.1.2/iterable_etl/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       22 2023-06-21 19:34:37.000000 iterable_etl-0.1.2/iterable_etl/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      155 2023-06-21 16:51:38.000000 iterable_etl-0.1.2/iterable_etl/__main__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1006 2023-06-21 18:38:35.000000 iterable_etl-0.1.2/iterable_etl/iterable_etl.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 19:34:48.560997 iterable_etl-0.1.2/iterable_etl/libs/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.2/iterable_etl/libs/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      667 2023-06-21 18:38:35.000000 iterable_etl-0.1.2/iterable_etl/libs/cnst.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1629 2023-06-21 16:51:38.000000 iterable_etl-0.1.2/iterable_etl/libs/dbg.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1086 2023-06-21 17:16:40.000000 iterable_etl-0.1.2/iterable_etl/libs/network.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1403 2023-06-21 18:38:35.000000 iterable_etl-0.1.2/iterable_etl/libs/spark.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      928 2023-06-21 16:51:38.000000 iterable_etl-0.1.2/iterable_etl/libs/transform.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 19:34:48.560997 iterable_etl-0.1.2/iterable_etl/tables/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.2/iterable_etl/tables/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      843 2023-06-21 17:33:07.000000 iterable_etl-0.1.2/iterable_etl/tables/campaign_history.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1370 2023-06-21 16:51:38.000000 iterable_etl-0.1.2/iterable_etl/tables/campaign_list_history.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1723 2023-06-21 16:51:38.000000 iterable_etl-0.1.2/iterable_etl/tables/campaign_metrics.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      769 2023-06-21 16:51:38.000000 iterable_etl-0.1.2/iterable_etl/tables/list.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2193 2023-06-21 19:33:53.000000 iterable_etl-0.1.2/iterable_etl/tables/list_user_history.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 19:34:48.556997 iterable_etl-0.1.2/iterable_etl.egg-info/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-21 19:34:48.000000 iterable_etl-0.1.2/iterable_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      717 2023-06-21 19:34:48.000000 iterable_etl-0.1.2/iterable_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-21 19:34:48.000000 iterable_etl-0.1.2/iterable_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       75 2023-06-21 19:34:48.000000 iterable_etl-0.1.2/iterable_etl.egg-info/requires.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       13 2023-06-21 19:34:48.000000 iterable_etl-0.1.2/iterable_etl.egg-info/top_level.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      426 2023-06-21 19:34:48.560997 iterable_etl-0.1.2/setup.cfg
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1050 2023-06-21 19:34:37.000000 iterable_etl-0.1.2/setup.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 19:34:48.560997 iterable_etl-0.1.2/tests/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.2/tests/__init__.py
```

### Comparing `iterable_etl-0.1.1/PKG-INFO` & `iterable_etl-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable_etl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.1.1/README_PUBLIC.md` & `iterable_etl-0.1.2/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/iterable_etl.py` & `iterable_etl-0.1.2/iterable_etl/iterable_etl.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/libs/cnst.py` & `iterable_etl-0.1.2/iterable_etl/libs/cnst.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/libs/dbg.py` & `iterable_etl-0.1.2/iterable_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/libs/network.py` & `iterable_etl-0.1.2/iterable_etl/libs/network.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/libs/spark.py` & `iterable_etl-0.1.2/iterable_etl/libs/spark.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/libs/transform.py` & `iterable_etl-0.1.2/iterable_etl/libs/transform.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/tables/campaign_history.py` & `iterable_etl-0.1.2/iterable_etl/tables/campaign_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/tables/campaign_list_history.py` & `iterable_etl-0.1.2/iterable_etl/tables/campaign_list_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/tables/campaign_metrics.py` & `iterable_etl-0.1.2/iterable_etl/tables/campaign_metrics.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/tables/list.py` & `iterable_etl-0.1.2/iterable_etl/tables/list.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/iterable_etl/tables/list_user_history.py` & `iterable_etl-0.1.2/iterable_etl/tables/list_user_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from iterable_etl.libs.transform import clean_column_headers, csv_to_dataframe
 
 
 def get_list_ids(api_url: str, headers: Dict[str, str]) -> List[Any]:
     """Make a GET request to the Iterable API and return a dictionary of list data."""
     data = get_data_json(api_url, headers)
     list_ids = [_list["id"] for _list in data["lists"]]
+    list_ids.sort()
     return list_ids
 
 
 def default_diff_writer():
     dbg("no diff writer")
 
 
@@ -42,23 +43,32 @@
     list_user_history_url = urls["lists_get_users"]
 
     df = pd.DataFrame()
 
     list_ids = get_list_ids(urls["lists"], get_headers())
 
     for i, list_id in enumerate(list_ids):
-        dbg("user list for list id {} of {}".format(i, len(list_ids)))
+        dbg(
+            "user list for list id {} of {}, list_id= {}".format(
+                i, len(list_ids), list_id
+            )
+        )
         url = f"{list_user_history_url}{list_id}"
 
         response_text = get_data_text(url, get_headers())
 
         time.sleep(13)
 
         if response_text:
+            dbg("list_id={} has content".format(list_id))
             _df = csv_to_dataframe(response_text)
             _df = _df.rename(columns={_df.columns[0]: "user_email"})
             _df["list_id"] = list_id
-            if spark & target_schema_table_name & diff_writer:
+            if (
+                spark is not None
+                and target_schema_table_name is not None
+                and diff_writer is not None
+            ):
                 diff_writer(spark, _df, target_schema_table_name)
             df = pd.concat([df, _df])
 
     return df
```

### Comparing `iterable_etl-0.1.1/iterable_etl.egg-info/PKG-INFO` & `iterable_etl-0.1.2/iterable_etl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable-etl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.1.1/iterable_etl.egg-info/SOURCES.txt` & `iterable_etl-0.1.2/iterable_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.1/setup.py` & `iterable_etl-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="iterable_etl",
-    version="0.1.1",
+    version="0.1.2",
     description="Replicate iterable data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

