# Comparing `tmp/pillar1-0.1.6.1.tar.gz` & `tmp/pillar1-0.1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.6.1.tar", last modified: Tue Jun 20 23:46:53 2023, max compression
+gzip compressed data, was "pillar1-0.1.6.2.tar", last modified: Tue Jun 20 23:48:14 2023, max compression
```

## Comparing `pillar1-0.1.6.1.tar` & `pillar1-0.1.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:46:53.018273 pillar1-0.1.6.1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:46:53.018107 pillar1-0.1.6.1/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.6.1/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:46:53.016488 pillar1-0.1.6.1/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.6.1/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3056 2023-06-20 23:45:57.000000 pillar1-0.1.6.1/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:46:53.017875 pillar1-0.1.6.1/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:46:52.000000 pillar1-0.1.6.1/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 23:46:52.000000 pillar1-0.1.6.1/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 23:46:52.000000 pillar1-0.1.6.1/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 23:46:52.000000 pillar1-0.1.6.1/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 23:46:53.018329 pillar1-0.1.6.1/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 23:45:10.000000 pillar1-0.1.6.1/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:48:14.386813 pillar1-0.1.6.2/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:48:14.386678 pillar1-0.1.6.2/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.6.2/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:48:14.385925 pillar1-0.1.6.2/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.6.2/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3047 2023-06-20 23:48:06.000000 pillar1-0.1.6.2/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:48:14.386490 pillar1-0.1.6.2/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:48:14.000000 pillar1-0.1.6.2/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 23:48:14.000000 pillar1-0.1.6.2/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 23:48:14.000000 pillar1-0.1.6.2/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 23:48:14.000000 pillar1-0.1.6.2/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 23:48:14.386856 pillar1-0.1.6.2/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 23:48:12.000000 pillar1-0.1.6.2/setup.py
```

### Comparing `pillar1-0.1.6.1/PKG-INFO` & `pillar1-0.1.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.6.1
+Version: 0.1.6.2
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.6.1/README.md` & `pillar1-0.1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.6.1/pillar1/pillar1.py` & `pillar1-0.1.6.2/pillar1/pillar1.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             response = self.client.invoke_endpoint(
                 EndpointName=self.end_point,
                 ContentType='application/json',
                 Body=json.dumps(payload)
             )
 
             self.response = json.loads(response['Body'].read())[0]['generated_text']
-            print(self.response)
+            self.code()
 
         if prompt:
             self.prompt = prompt
             submit_request(self.prompt)
         else:
             textarea_bg = widgets.Textarea(description='Provide any necessary background:', layout=widgets.Layout(width='80%', height='200px'),
                                            style={'description_width': 'initial'})
```

### Comparing `pillar1-0.1.6.1/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.6.2/pillar1.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.6.1
+Version: 0.1.6.2
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.6.1/setup.py` & `pillar1-0.1.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.6.1',
+    version='0.1.6.2',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

