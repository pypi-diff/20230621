# Comparing `tmp/pillar1-0.1.5.8.tar.gz` & `tmp/pillar1-0.1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.5.8.tar", last modified: Tue Jun 20 23:11:52 2023, max compression
+gzip compressed data, was "pillar1-0.1.5.9.tar", last modified: Tue Jun 20 23:27:54 2023, max compression
```

## Comparing `pillar1-0.1.5.8.tar` & `pillar1-0.1.5.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:11:52.895860 pillar1-0.1.5.8/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:11:52.895725 pillar1-0.1.5.8/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.8/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:11:52.894846 pillar1-0.1.5.8/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.8/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2459 2023-06-20 23:11:41.000000 pillar1-0.1.5.8/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:11:52.895519 pillar1-0.1.5.8/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:11:52.000000 pillar1-0.1.5.8/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 23:11:52.000000 pillar1-0.1.5.8/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 23:11:52.000000 pillar1-0.1.5.8/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 23:11:52.000000 pillar1-0.1.5.8/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 23:11:52.895901 pillar1-0.1.5.8/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 23:11:48.000000 pillar1-0.1.5.8/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:27:54.991294 pillar1-0.1.5.9/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:27:54.991160 pillar1-0.1.5.9/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.9/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:27:54.990174 pillar1-0.1.5.9/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.9/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2762 2023-06-20 23:25:32.000000 pillar1-0.1.5.9/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:27:54.990925 pillar1-0.1.5.9/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:27:54.000000 pillar1-0.1.5.9/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 23:27:54.000000 pillar1-0.1.5.9/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 23:27:54.000000 pillar1-0.1.5.9/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 23:27:54.000000 pillar1-0.1.5.9/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 23:27:54.991350 pillar1-0.1.5.9/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 23:27:52.000000 pillar1-0.1.5.9/setup.py
```

### Comparing `pillar1-0.1.5.8/PKG-INFO` & `pillar1-0.1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.8
+Version: 0.1.5.9
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.8/README.md` & `pillar1-0.1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.8/pillar1/pillar1.py` & `pillar1-0.1.5.9/pillar1/pillar1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import json
 import boto3
 import ipywidgets as widgets
 from IPython.display import display
+from pyspark.sql import SparkSession
 
 
 class Model:
     def __init__(self, user_name: str = '', password: str = '', end_point: str = '', max_new_tokens: int = 200):
         self.end_point = end_point
         self.prompt = None
+        self.result = None
+        self.cleaned_code = ''
         self.response = None
         self.max_new_tokens = max_new_tokens
 
         self.client = boto3.client(
             'sagemaker-runtime',
             aws_access_key_id=user_name,
             aws_secret_access_key=password,
             region_name='us-west-2'
         )
 
     def code(self):
-        cleaned_code = self.response.replace(self.prompt, '')
-        print(cleaned_code)
+        self.cleaned_code = self.response.replace(self.prompt, '').strip()
+        print(self.cleaned_code)
+
+    def execute(self):
+        spark = SparkSession.builder.getOrCreate()
+        self.result = spark.sql(self.cleaned_code)
+        self.result.show()
 
     def query(self, prompt: str = ''):
         def submit_request(prompt):
             payload = {
                 'inputs': prompt,
                 "parameters": {
                     "do_sample": True,
@@ -57,11 +65,12 @@
             display(textarea_bg)
             display(input_text)
             display(button)
 
             # Define button click event
             def submit_button(b):
                 prompt = f"Given this background:\n\"{textarea_bg.value}\"\n\nAnswer this question: \"{input_text.value}\""
+                self.prompt = prompt
                 submit_request(prompt)
 
             # Bind button click event to function
             button.on_click(submit_button)
```

### Comparing `pillar1-0.1.5.8/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.5.9/pillar1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.8
+Version: 0.1.5.9
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.8/setup.py` & `pillar1-0.1.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.5.8',
+    version='0.1.5.9',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

