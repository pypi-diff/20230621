# Comparing `tmp/arcanum-newspaper-segmentation-client-1.7.0.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.7.0.tar", last modified: Wed Jun 21 13:26:05 2023, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.7.1.tar", last modified: Wed Jun 21 13:49:15 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.7.0.tar` & `arcanum-newspaper-segmentation-client-1.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:26:05.150183 arcanum-newspaper-segmentation-client-1.7.0/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.0/LICENSE
--rw-rw-rw-   0        0        0      675 2023-06-21 13:26:05.149185 arcanum-newspaper-segmentation-client-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.0/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 13:26:05.150183 arcanum-newspaper-segmentation-client-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-06-21 13:25:09.000000 arcanum-newspaper-segmentation-client-1.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:26:05.102311 arcanum-newspaper-segmentation-client-1.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 13:26:05.125249 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      675 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 13:26:05.148188 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    13524 2023-04-18 10:48:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0     3089 2023-06-21 11:14:42.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/pdf.py
--rw-rw-rw-   0        0        0      756 2023-04-18 08:06:36.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/text.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:49:15.352976 arcanum-newspaper-segmentation-client-1.7.1/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-06-21 13:49:15.351979 arcanum-newspaper-segmentation-client-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.1/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:49:15.352976 arcanum-newspaper-segmentation-client-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-06-21 13:48:58.000000 arcanum-newspaper-segmentation-client-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:49:15.325059 arcanum-newspaper-segmentation-client-1.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 13:49:15.345020 arcanum-newspaper-segmentation-client-1.7.1/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-06-21 13:49:15.000000 arcanum-newspaper-segmentation-client-1.7.1/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-06-21 13:49:15.000000 arcanum-newspaper-segmentation-client-1.7.1/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:49:15.000000 arcanum-newspaper-segmentation-client-1.7.1/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-21 13:49:15.000000 arcanum-newspaper-segmentation-client-1.7.1/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-06-21 13:49:15.000000 arcanum-newspaper-segmentation-client-1.7.1/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 13:49:15.350981 arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    13524 2023-04-18 10:48:05.000000 arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     3143 2023-06-21 13:48:13.000000 arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      756 2023-04-18 08:06:36.000000 arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/text.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/LICENSE` & `arcanum-newspaper-segmentation-client-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.7.0
+Version: 1.7.1
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/setup.py` & `arcanum-newspaper-segmentation-client-1.7.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.7.0",
+    version="1.7.1",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
```

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.7.1/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.7.0
+Version: 1.7.1
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt` & `arcanum-newspaper-segmentation-client-1.7.1/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/__init__.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/clip.py` & `arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/clip.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/pdf.py` & `arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
             }
         }]
     }
     page_text = page.get_text("dict")
     line_id = 2
     line_ids = []
     for block in page_text["blocks"]:
+        if block["type"] != 0:
+            continue
         for line in block["lines"]:
             line_text = "".join(span["text"] for span in line["spans"])
             if not line_text:
                 continue
             image_box = page.bound()
             textract_bounding_box = bbox_to_textract_bounding_box(line["bbox"], image_box)
             x_min, y_min, x_max, y_max = textract_bounding_box["Left"], textract_bounding_box["Top"], \
```

### Comparing `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/text.py` & `arcanum-newspaper-segmentation-client-1.7.1/src/newspaper_segmentation_client/text.py`

 * *Files identical despite different names*

