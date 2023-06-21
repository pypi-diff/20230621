# Comparing `tmp/cipher_kit-0.0.1.tar.gz` & `tmp/cipher_kit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipher_kit-0.0.1.tar", last modified: Wed Jun 21 06:16:22 2023, max compression
+gzip compressed data, was "cipher_kit-0.0.2.tar", last modified: Wed Jun 21 06:21:15 2023, max compression
```

## Comparing `cipher_kit-0.0.1.tar` & `cipher_kit-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 06:16:22.240206 cipher_kit-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-06-20 06:27:52.000000 cipher_kit-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1772 2023-06-21 06:16:22.239205 cipher_kit-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 06:16:22.219202 cipher_kit-0.0.1/app/
-drwxrwxrwx   0        0        0        0 2023-06-21 06:16:22.237199 cipher_kit-0.0.1/app/cipher_kit.egg-info/
--rw-rw-rw-   0        0        0     1772 2023-06-21 06:16:21.000000 cipher_kit-0.0.1/app/cipher_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-06-21 06:16:21.000000 cipher_kit-0.0.1/app/cipher_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 06:16:21.000000 cipher_kit-0.0.1/app/cipher_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 06:16:21.000000 cipher_kit-0.0.1/app/cipher_kit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 06:16:22.241209 cipher_kit-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-21 06:16:02.000000 cipher_kit-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:21:15.629607 cipher_kit-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-20 06:27:52.000000 cipher_kit-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1772 2023-06-21 06:21:15.628608 cipher_kit-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 06:21:15.611492 cipher_kit-0.0.2/app/
+drwxrwxrwx   0        0        0        0 2023-06-21 06:21:15.626488 cipher_kit-0.0.2/app/cipher_kit.egg-info/
+-rw-rw-rw-   0        0        0     1772 2023-06-21 06:21:15.000000 cipher_kit-0.0.2/app/cipher_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-06-21 06:21:15.000000 cipher_kit-0.0.2/app/cipher_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 06:21:15.000000 cipher_kit-0.0.2/app/cipher_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-21 06:21:15.000000 cipher_kit-0.0.2/app/cipher_kit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 06:21:15.629607 cipher_kit-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-06-21 06:18:26.000000 cipher_kit-0.0.2/setup.py
```

### Comparing `cipher_kit-0.0.1/LICENSE.txt` & `cipher_kit-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cipher_kit-0.0.1/PKG-INFO` & `cipher_kit-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipher_kit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Module which helps in encryption and decryption
 Home-page: https://github.com/PankajVishw50/cipher_kit
 Author: Pankaj
 Author-email: pankaj.vishw.dev@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cipher_kit-0.0.1/app/cipher_kit.egg-info/PKG-INFO` & `cipher_kit-0.0.2/app/cipher_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipher-kit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Module which helps in encryption and decryption
 Home-page: https://github.com/PankajVishw50/cipher_kit
 Author: Pankaj
 Author-email: pankaj.vishw.dev@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cipher_kit-0.0.1/setup.py` & `cipher_kit-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from setuptools import setup
 
 with open("app/Readme.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="cipher_kit",
-    version="0.0.1",
+    version="0.0.2",
     description="Module which helps in encryption and decryption",
     author="Pankaj",
     author_email="pankaj.vishw.dev@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PankajVishw50/cipher_kit",
     py_modules=["cipher_kit"],
     package_dir={"": "app"},
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 ",
         "License :: OSI Approved :: MIT License"
 
-    ]
+    ],
+    extra_requires={
+        "dev": [
+            "pytest>=7.0.0",
+        ]
+    }
+
 )
```

