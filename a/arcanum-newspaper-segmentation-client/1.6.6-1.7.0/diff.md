# Comparing `tmp/arcanum-newspaper-segmentation-client-1.6.6.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.6.tar", last modified: Mon Apr 17 15:59:58 2023, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.7.0.tar", last modified: Wed Jun 21 13:26:05 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.6.6.tar` & `arcanum-newspaper-segmentation-client-1.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:59:58.781078 arcanum-newspaper-segmentation-client-1.6.6/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.6/LICENSE
--rw-rw-rw-   0        0        0      675 2023-04-17 15:59:58.780080 arcanum-newspaper-segmentation-client-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.6/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 15:59:58.781078 arcanum-newspaper-segmentation-client-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-17 15:59:41.000000 arcanum-newspaper-segmentation-client-1.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:59:58.736198 arcanum-newspaper-segmentation-client-1.6.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 15:59:58.757141 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      675 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 15:59:58.780080 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    13521 2023-04-17 15:58:20.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0     3203 2023-04-14 10:21:05.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/pdf.py
--rw-rw-rw-   0        0        0      756 2023-04-14 14:44:20.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/text.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:26:05.150183 arcanum-newspaper-segmentation-client-1.7.0/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-06-21 13:26:05.149185 arcanum-newspaper-segmentation-client-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.0/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:26:05.150183 arcanum-newspaper-segmentation-client-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-06-21 13:25:09.000000 arcanum-newspaper-segmentation-client-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:26:05.102311 arcanum-newspaper-segmentation-client-1.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 13:26:05.125249 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-06-21 13:26:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 13:26:05.148188 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    13524 2023-04-18 10:48:05.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     3089 2023-06-21 11:14:42.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      756 2023-04-18 08:06:36.000000 arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/text.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/LICENSE` & `arcanum-newspaper-segmentation-client-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.6
+Version: 1.7.0
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/setup.py` & `arcanum-newspaper-segmentation-client-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.6.6",
+    version="1.7.0",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.6
+Version: 1.7.0
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt` & `arcanum-newspaper-segmentation-client-1.7.0/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 
     response = requests.get("https://api.arcanum.com/v1/newspaper-segmentation/analyze-page",
                             data=json.dumps(request_data), headers={"x-api-key": api_key})
 
     if response.status_code != 200:
         if response.status_code == 400:
             raise RuntimeError(response.json()["error"])
-        raise RuntimeError("Error during API call")
+        raise RuntimeError(response.json()["message"])
 
     segmented_page = response.json()
     add_ocr_blocks(segmented_page, textract_response)
     return segmented_page
 
 
 def run_newspaper_segmentation_without_textract(image: BinaryIO, textract_response, api_key: str):
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/clip.py` & `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/clip.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/pdf.py` & `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Dict, Tuple
-import io
 
 from PIL import Image
 import fitz
 
 from newspaper_segmentation_client import run_newspaper_segmentation_on_image
 
 
@@ -30,16 +29,15 @@
             'Id': '1',
             'Geometry': {
                 'BoundingBox': {"Width": 1.0, "Height": 1.0, "Top": 0.0, "Left": 0.0},
                 'Polygon': [{'X': 0.0, 'Y': 0.0}, {'X': 1.0, 'Y': 0.0}, {'X': 1.0, 'Y': 1.0}, {'X': 0.0, 'Y': 1.0}]
             }
         }]
     }
-    text_page_flags = fitz.TEXT_INHIBIT_SPACES | fitz.TEXT_PRESERVE_WHITESPACE
-    page_text = page.get_text("dict", flags=text_page_flags)
+    page_text = page.get_text("dict")
     line_id = 2
     line_ids = []
     for block in page_text["blocks"]:
         for line in block["lines"]:
             line_text = "".join(span["text"] for span in line["spans"])
             if not line_text:
                 continue
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/text.py` & `arcanum-newspaper-segmentation-client-1.7.0/src/newspaper_segmentation_client/text.py`

 * *Files identical despite different names*

