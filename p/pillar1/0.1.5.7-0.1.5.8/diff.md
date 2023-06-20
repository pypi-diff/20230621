# Comparing `tmp/pillar1-0.1.5.7.tar.gz` & `tmp/pillar1-0.1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.5.7.tar", last modified: Tue Jun 20 21:36:06 2023, max compression
+gzip compressed data, was "pillar1-0.1.5.8.tar", last modified: Tue Jun 20 23:11:52 2023, max compression
```

## Comparing `pillar1-0.1.5.7.tar` & `pillar1-0.1.5.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 21:36:06.267908 pillar1-0.1.5.7/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 21:36:06.267776 pillar1-0.1.5.7/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.7/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 21:36:06.266893 pillar1-0.1.5.7/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.7/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2348 2023-06-20 21:33:54.000000 pillar1-0.1.5.7/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 21:36:06.267550 pillar1-0.1.5.7/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 21:36:06.000000 pillar1-0.1.5.7/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 21:36:06.000000 pillar1-0.1.5.7/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 21:36:06.000000 pillar1-0.1.5.7/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 21:36:06.000000 pillar1-0.1.5.7/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 21:36:06.267950 pillar1-0.1.5.7/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 21:34:02.000000 pillar1-0.1.5.7/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:11:52.895860 pillar1-0.1.5.8/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:11:52.895725 pillar1-0.1.5.8/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.8/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:11:52.894846 pillar1-0.1.5.8/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.8/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2459 2023-06-20 23:11:41.000000 pillar1-0.1.5.8/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:11:52.895519 pillar1-0.1.5.8/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:11:52.000000 pillar1-0.1.5.8/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 23:11:52.000000 pillar1-0.1.5.8/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 23:11:52.000000 pillar1-0.1.5.8/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 23:11:52.000000 pillar1-0.1.5.8/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 23:11:52.895901 pillar1-0.1.5.8/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 23:11:48.000000 pillar1-0.1.5.8/setup.py
```

### Comparing `pillar1-0.1.5.7/PKG-INFO` & `pillar1-0.1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.7
+Version: 0.1.5.8
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.7/README.md` & `pillar1-0.1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.7/pillar1/pillar1.py` & `pillar1-0.1.5.8/pillar1/pillar1.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,18 @@
         self.client = boto3.client(
             'sagemaker-runtime',
             aws_access_key_id=user_name,
             aws_secret_access_key=password,
             region_name='us-west-2'
         )
 
+    def code(self):
+        cleaned_code = self.response.replace(self.prompt, '')
+        print(cleaned_code)
+
     def query(self, prompt: str = ''):
         def submit_request(prompt):
             payload = {
                 'inputs': prompt,
                 "parameters": {
                     "do_sample": True,
                     "top_p": 0.7,
```

### Comparing `pillar1-0.1.5.7/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.5.8/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.7
+Version: 0.1.5.8
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.7/setup.py` & `pillar1-0.1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.5.7',
+    version='0.1.5.8',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

