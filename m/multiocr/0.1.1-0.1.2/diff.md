# Comparing `tmp/multiocr-0.1.1.tar.gz` & `tmp/multiocr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiocr-0.1.1.tar", max compression
+gzip compressed data, was "multiocr-0.1.2.tar", max compression
```

## Comparing `multiocr-0.1.1.tar` & `multiocr-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2647 2023-06-19 22:06:37.927399 multiocr-0.1.1/README.md
--rw-r--r--   0        0        0       35 2023-06-10 13:04:19.610231 multiocr-0.1.1/multiocr/__init__.py
--rw-r--r--   0        0        0      338 2023-06-19 22:04:10.847491 multiocr-0.1.1/multiocr/base_class.py
--rw-r--r--   0        0        0     2276 2023-06-19 21:54:01.164972 multiocr-0.1.1/multiocr/main.py
--rw-r--r--   0        0        0      202 2023-06-19 21:48:38.816200 multiocr-0.1.1/multiocr/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 04:58:23.910390 multiocr-0.1.1/multiocr/pipelines/aws_textract/__init__.py
--rw-r--r--   0        0        0     4383 2023-06-19 22:00:05.907425 multiocr-0.1.1/multiocr/pipelines/aws_textract/engine.py
--rw-r--r--   0        0        0     2535 2023-06-19 21:57:53.639183 multiocr-0.1.1/multiocr/pipelines/easy_ocr/engine.py
--rw-r--r--   0        0        0        0 2023-06-10 04:58:45.721303 multiocr-0.1.1/multiocr/pipelines/paddle_ocr/__init__.py
--rw-r--r--   0        0        0     2707 2023-06-19 21:58:41.369725 multiocr-0.1.1/multiocr/pipelines/paddle_ocr/engine.py
--rw-r--r--   0        0        0        0 2023-06-10 04:55:24.885038 multiocr-0.1.1/multiocr/pipelines/tesseract/__init__.py
--rw-r--r--   0        0        0     3399 2023-06-19 21:58:52.558658 multiocr-0.1.1/multiocr/pipelines/tesseract/engine.py
--rw-r--r--   0        0        0     1319 2023-06-10 08:55:37.312478 multiocr-0.1.1/multiocr/utils.py
--rw-r--r--   0        0        0      378 2023-06-19 22:08:12.037212 multiocr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 multiocr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2647 2023-06-19 22:14:53.371351 multiocr-0.1.2/README.md
+-rw-r--r--   0        0        0       35 2023-06-10 13:04:19.610231 multiocr-0.1.2/multiocr/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-19 22:04:10.847491 multiocr-0.1.2/multiocr/base_class.py
+-rw-r--r--   0        0        0     2276 2023-06-21 01:06:27.978422 multiocr-0.1.2/multiocr/main.py
+-rw-r--r--   0        0        0      202 2023-06-19 21:48:38.816200 multiocr-0.1.2/multiocr/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 04:58:23.910390 multiocr-0.1.2/multiocr/pipelines/aws_textract/__init__.py
+-rw-r--r--   0        0        0     4383 2023-06-19 22:00:05.907425 multiocr-0.1.2/multiocr/pipelines/aws_textract/engine.py
+-rw-r--r--   0        0        0     2535 2023-06-19 21:57:53.639183 multiocr-0.1.2/multiocr/pipelines/easy_ocr/engine.py
+-rw-r--r--   0        0        0        0 2023-06-10 04:58:45.721303 multiocr-0.1.2/multiocr/pipelines/paddle_ocr/__init__.py
+-rw-r--r--   0        0        0     2707 2023-06-19 21:58:41.369725 multiocr-0.1.2/multiocr/pipelines/paddle_ocr/engine.py
+-rw-r--r--   0        0        0        0 2023-06-10 04:55:24.885038 multiocr-0.1.2/multiocr/pipelines/tesseract/__init__.py
+-rw-r--r--   0        0        0     3405 2023-06-21 01:17:26.126369 multiocr-0.1.2/multiocr/pipelines/tesseract/engine.py
+-rw-r--r--   0        0        0     1319 2023-06-10 08:55:37.312478 multiocr-0.1.2/multiocr/utils.py
+-rw-r--r--   0        0        0      378 2023-06-21 01:21:53.829613 multiocr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 multiocr-0.1.2/PKG-INFO
```

### Comparing `multiocr-0.1.1/README.md` & `multiocr-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.1/multiocr/main.py` & `multiocr-0.1.2/multiocr/main.py`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.1/multiocr/pipelines/aws_textract/engine.py` & `multiocr-0.1.2/multiocr/pipelines/aws_textract/engine.py`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.1/multiocr/pipelines/easy_ocr/engine.py` & `multiocr-0.1.2/multiocr/pipelines/easy_ocr/engine.py`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.1/multiocr/pipelines/paddle_ocr/engine.py` & `multiocr-0.1.2/multiocr/pipelines/paddle_ocr/engine.py`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.1/multiocr/pipelines/tesseract/engine.py` & `multiocr-0.1.2/multiocr/pipelines/tesseract/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     text_extraction(): This method extracts text from the image using Tesseract OCR and returns the text as a dictionary with the block IDs as keys and the text, confidence score, and bounding box coordinates as values.
     text_extraction_to_json(text_dict): This method takes the dictionary output from text_extraction() as input and saves it to a JSON file.
     text_extraction_to_df(text_dict): This method takes the dictionary output from text_extraction() as input and saves it to a Pandas DataFrame with columns for the text, confidence score, and bounding box coordinates.
     extract_plain_text(text_dict): This method takes the dictionary output from text_extraction() as input and saves the plain text to a text file.
     """
     def __init__(self, config:Union[dict, None]=None):
         self.config = config
-        self.config.pop("output_type")
+        self.config.pop("output_type", None)
     
     def text_extraction(self, image_file):
         try:
             text = pytesseract.image_to_data( Image.open(image_file), output_type='dict', **self.config)
             self.raw_ocr = text
         except Exception as e:
             raise Exception(f"Error detecting text in image: {e}")
```

### Comparing `multiocr-0.1.1/multiocr/utils.py` & `multiocr-0.1.2/multiocr/utils.py`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.1/PKG-INFO` & `multiocr-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiocr
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Aravindh
 Author-email: 32878238+s-aravindh@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

