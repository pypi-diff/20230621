# Comparing `tmp/cipher_kit-0.0.2.tar.gz` & `tmp/cipher_kit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipher_kit-0.0.2.tar", last modified: Wed Jun 21 06:21:15 2023, max compression
+gzip compressed data, was "cipher_kit-0.0.3.tar", last modified: Wed Jun 21 07:56:49 2023, max compression
```

## Comparing `cipher_kit-0.0.2.tar` & `cipher_kit-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 06:21:15.629607 cipher_kit-0.0.2/
--rw-rw-rw-   0        0        0     1082 2023-06-20 06:27:52.000000 cipher_kit-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1772 2023-06-21 06:21:15.628608 cipher_kit-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 06:21:15.611492 cipher_kit-0.0.2/app/
-drwxrwxrwx   0        0        0        0 2023-06-21 06:21:15.626488 cipher_kit-0.0.2/app/cipher_kit.egg-info/
--rw-rw-rw-   0        0        0     1772 2023-06-21 06:21:15.000000 cipher_kit-0.0.2/app/cipher_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-06-21 06:21:15.000000 cipher_kit-0.0.2/app/cipher_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 06:21:15.000000 cipher_kit-0.0.2/app/cipher_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 06:21:15.000000 cipher_kit-0.0.2/app/cipher_kit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 06:21:15.629607 cipher_kit-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-06-21 06:18:26.000000 cipher_kit-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.076026 cipher_kit-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2023-06-20 06:27:52.000000 cipher_kit-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1772 2023-06-21 07:56:49.074018 cipher_kit-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.048018 cipher_kit-0.0.3/app/
+drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.055020 cipher_kit-0.0.3/app/cipher_kit/
+-rw-rw-rw-   0        0        0       34 2023-06-20 05:32:57.000000 cipher_kit-0.0.3/app/cipher_kit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.066027 cipher_kit-0.0.3/app/cipher_kit/src/
+-rw-rw-rw-   0        0        0        0 2023-06-19 17:14:24.000000 cipher_kit-0.0.3/app/cipher_kit/src/__init__.py
+-rw-rw-rw-   0        0        0     2475 2023-06-20 07:03:22.000000 cipher_kit-0.0.3/app/cipher_kit/src/cipher.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.071020 cipher_kit-0.0.3/app/cipher_kit/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-20 05:48:41.000000 cipher_kit-0.0.3/app/cipher_kit/tests/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-06-20 07:16:55.000000 cipher_kit-0.0.3/app/cipher_kit/tests/test_cipher.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.063022 cipher_kit-0.0.3/app/cipher_kit.egg-info/
+-rw-rw-rw-   0        0        0     1772 2023-06-21 07:56:48.000000 cipher_kit-0.0.3/app/cipher_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-21 07:56:48.000000 cipher_kit-0.0.3/app/cipher_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 07:56:48.000000 cipher_kit-0.0.3/app/cipher_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-21 07:56:48.000000 cipher_kit-0.0.3/app/cipher_kit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 07:56:49.076026 cipher_kit-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      795 2023-06-21 07:45:14.000000 cipher_kit-0.0.3/setup.py
```

### Comparing `cipher_kit-0.0.2/LICENSE.txt` & `cipher_kit-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cipher_kit-0.0.2/PKG-INFO` & `cipher_kit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipher_kit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Module which helps in encryption and decryption
 Home-page: https://github.com/PankajVishw50/cipher_kit
 Author: Pankaj
 Author-email: pankaj.vishw.dev@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cipher_kit-0.0.2/app/cipher_kit.egg-info/PKG-INFO` & `cipher_kit-0.0.3/app/cipher_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipher-kit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Module which helps in encryption and decryption
 Home-page: https://github.com/PankajVishw50/cipher_kit
 Author: Pankaj
 Author-email: pankaj.vishw.dev@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cipher_kit-0.0.2/setup.py` & `cipher_kit-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("app/Readme.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="cipher_kit",
-    version="0.0.2",
+    version="0.0.3",
     description="Module which helps in encryption and decryption",
     author="Pankaj",
     author_email="pankaj.vishw.dev@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PankajVishw50/cipher_kit",
-    py_modules=["cipher_kit"],
+    packages=find_packages("app"),
     package_dir={"": "app"},
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 ",
         "License :: OSI Approved :: MIT License"
 
     ],
```

