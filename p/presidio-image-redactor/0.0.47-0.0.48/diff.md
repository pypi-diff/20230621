# Comparing `tmp/presidio_image_redactor-0.0.47-py3-none-any.whl.zip` & `tmp/presidio_image_redactor-0.0.48-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 23535 bytes, number of entries: 17
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-04 10:03 presidio_image_redactor/__init__.py
--rw-r--r--  2.0 unx     4970 b- defN 23-Jun-04 10:03 presidio_image_redactor/bbox.py
--rw-r--r--  2.0 unx    10224 b- defN 23-Jun-04 10:03 presidio_image_redactor/dicom_image_pii_verify_engine.py
--rw-r--r--  2.0 unx    32055 b- defN 23-Jun-04 10:03 presidio_image_redactor/dicom_image_redactor_engine.py
--rw-r--r--  2.0 unx     6921 b- defN 23-Jun-04 10:03 presidio_image_redactor/image_analyzer_engine.py
--rw-r--r--  2.0 unx     2470 b- defN 23-Jun-04 10:03 presidio_image_redactor/image_pii_verify_engine.py
--rw-r--r--  2.0 unx     1818 b- defN 23-Jun-04 10:03 presidio_image_redactor/image_redactor_engine.py
--rw-r--r--  2.0 unx      981 b- defN 23-Jun-04 10:03 presidio_image_redactor/ocr.py
--rw-r--r--  2.0 unx      615 b- defN 23-Jun-04 10:03 presidio_image_redactor/tesseract_ocr.py
--rw-r--r--  2.0 unx      216 b- defN 23-Jun-04 10:03 presidio_image_redactor/entities/__init__.py
--rw-r--r--  2.0 unx     2034 b- defN 23-Jun-04 10:03 presidio_image_redactor/entities/api_request_convertor.py
--rw-r--r--  2.0 unx     2106 b- defN 23-Jun-04 10:03 presidio_image_redactor/entities/image_recognizer_result.py
--rw-r--r--  2.0 unx      274 b- defN 23-Jun-04 10:03 presidio_image_redactor/entities/invalid_exception.py
--rw-r--r--  2.0 unx     6342 b- defN 23-Jun-04 10:03 presidio_image_redactor-0.0.47.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 10:03 presidio_image_redactor-0.0.47.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-04 10:03 presidio_image_redactor-0.0.47.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1709 b- defN 23-Jun-04 10:03 presidio_image_redactor-0.0.47.dist-info/RECORD
-17 files, 73635 bytes uncompressed, 20619 bytes compressed:  72.0%
+Zip file size: 23527 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-21 15:15 presidio_image_redactor/__init__.py
+-rw-r--r--  2.0 unx     4970 b- defN 23-Jun-21 15:15 presidio_image_redactor/bbox.py
+-rw-r--r--  2.0 unx    10224 b- defN 23-Jun-21 15:15 presidio_image_redactor/dicom_image_pii_verify_engine.py
+-rw-r--r--  2.0 unx    32055 b- defN 23-Jun-21 15:15 presidio_image_redactor/dicom_image_redactor_engine.py
+-rw-r--r--  2.0 unx     6921 b- defN 23-Jun-21 15:15 presidio_image_redactor/image_analyzer_engine.py
+-rw-r--r--  2.0 unx     2470 b- defN 23-Jun-21 15:15 presidio_image_redactor/image_pii_verify_engine.py
+-rw-r--r--  2.0 unx     1818 b- defN 23-Jun-21 15:15 presidio_image_redactor/image_redactor_engine.py
+-rw-r--r--  2.0 unx      981 b- defN 23-Jun-21 15:15 presidio_image_redactor/ocr.py
+-rw-r--r--  2.0 unx      615 b- defN 23-Jun-21 15:15 presidio_image_redactor/tesseract_ocr.py
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-21 15:15 presidio_image_redactor/entities/__init__.py
+-rw-r--r--  2.0 unx     2034 b- defN 23-Jun-21 15:15 presidio_image_redactor/entities/api_request_convertor.py
+-rw-r--r--  2.0 unx     2106 b- defN 23-Jun-21 15:15 presidio_image_redactor/entities/image_recognizer_result.py
+-rw-r--r--  2.0 unx      274 b- defN 23-Jun-21 15:15 presidio_image_redactor/entities/invalid_exception.py
+-rw-r--r--  2.0 unx     6311 b- defN 23-Jun-21 15:15 presidio_image_redactor-0.0.48.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 15:15 presidio_image_redactor-0.0.48.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-21 15:15 presidio_image_redactor-0.0.48.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1709 b- defN 23-Jun-21 15:15 presidio_image_redactor-0.0.48.dist-info/RECORD
+17 files, 73604 bytes uncompressed, 20611 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: presidio_image_redactor/entities/image_recognizer_result.py
 Comment: 
 
 Filename: presidio_image_redactor/entities/invalid_exception.py
 Comment: 
 
-Filename: presidio_image_redactor-0.0.47.dist-info/METADATA
+Filename: presidio_image_redactor-0.0.48.dist-info/METADATA
 Comment: 
 
-Filename: presidio_image_redactor-0.0.47.dist-info/WHEEL
+Filename: presidio_image_redactor-0.0.48.dist-info/WHEEL
 Comment: 
 
-Filename: presidio_image_redactor-0.0.47.dist-info/top_level.txt
+Filename: presidio_image_redactor-0.0.48.dist-info/top_level.txt
 Comment: 
 
-Filename: presidio_image_redactor-0.0.47.dist-info/RECORD
+Filename: presidio_image_redactor-0.0.48.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `presidio_image_redactor-0.0.47.dist-info/METADATA` & `presidio_image_redactor-0.0.48.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: presidio-image-redactor
-Version: 0.0.47
+Version: 0.0.48
 Summary: Presidio image redactor package
 Home-page: https://github.com/Microsoft/presidio
 License: MIT
 Keywords: presidio_image_redactor
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,18 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: pillow (>=9.0)
-Requires-Dist: pytesseract (==0.3.7)
+Requires-Dist: pytesseract (<0.4,>=0.3.7)
 Requires-Dist: presidio-analyzer (>=1.9.0)
-Requires-Dist: matplotlib (==3.6.2)
-Requires-Dist: pydantic (==1.7.4)
+Requires-Dist: matplotlib (>=3.6)
 Requires-Dist: pydicom (>=2.3.0)
 Requires-Dist: pypng (>=0.20220715.0)
 
 # Presidio Image Redactor
 
 ***Please notice, this package is still in alpha and not production ready.***
```

## Comparing `presidio_image_redactor-0.0.47.dist-info/RECORD` & `presidio_image_redactor-0.0.48.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 presidio_image_redactor/image_redactor_engine.py,sha256=z8n1LLr54Y9z-vHANNEeYj5x0j28fiy1WhnjG8UZNhI,1818
 presidio_image_redactor/ocr.py,sha256=n7x1JtH-fkbF8fvf2kRP2848JdXI59VPW4xJ3XOHj0o,981
 presidio_image_redactor/tesseract_ocr.py,sha256=cxnjsyaL3t6C8JJQe8tOslu8DeOZicnppEhUR3YEaG0,615
 presidio_image_redactor/entities/__init__.py,sha256=RqsxcYKASoFLPqPW5EmEoSIX85vraPFaUQdILQL2K_c,216
 presidio_image_redactor/entities/api_request_convertor.py,sha256=PAgB6aBAk5h1T749W5rLbWxrA80TPyo6U4BDq7Qzn90,2034
 presidio_image_redactor/entities/image_recognizer_result.py,sha256=9MR_KCXfJHqoawOQFixHMT_h1kSGBf5WlR9jnVJD1TI,2106
 presidio_image_redactor/entities/invalid_exception.py,sha256=FDGsHC0o5R06RmboBmqhFVYBfmole9TQvjziZw2eJ4w,274
-presidio_image_redactor-0.0.47.dist-info/METADATA,sha256=bXI5pIysESdA9FVC1iXW2tZlGqTe9C9Bxj5OFSfOwT4,6342
-presidio_image_redactor-0.0.47.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-presidio_image_redactor-0.0.47.dist-info/top_level.txt,sha256=exMcxj0mg3Ey4ACq-Chz4sD5_7z-Z1YqHcfmWYUr0Oo,24
-presidio_image_redactor-0.0.47.dist-info/RECORD,,
+presidio_image_redactor-0.0.48.dist-info/METADATA,sha256=mJgcUwdeRUyNSa31dfktvnC15_FyF-7beP1xxMQXMIQ,6311
+presidio_image_redactor-0.0.48.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+presidio_image_redactor-0.0.48.dist-info/top_level.txt,sha256=exMcxj0mg3Ey4ACq-Chz4sD5_7z-Z1YqHcfmWYUr0Oo,24
+presidio_image_redactor-0.0.48.dist-info/RECORD,,
```

