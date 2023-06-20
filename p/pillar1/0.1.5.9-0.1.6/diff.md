# Comparing `tmp/pillar1-0.1.5.9.tar.gz` & `tmp/pillar1-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.5.9.tar", last modified: Tue Jun 20 23:27:54 2023, max compression
+gzip compressed data, was "pillar1-0.1.6.tar", last modified: Tue Jun 20 23:33:58 2023, max compression
```

## Comparing `pillar1-0.1.5.9.tar` & `pillar1-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:27:54.991294 pillar1-0.1.5.9/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:27:54.991160 pillar1-0.1.5.9/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.9/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:27:54.990174 pillar1-0.1.5.9/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.9/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2762 2023-06-20 23:25:32.000000 pillar1-0.1.5.9/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:27:54.990925 pillar1-0.1.5.9/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:27:54.000000 pillar1-0.1.5.9/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 23:27:54.000000 pillar1-0.1.5.9/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 23:27:54.000000 pillar1-0.1.5.9/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 23:27:54.000000 pillar1-0.1.5.9/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 23:27:54.991350 pillar1-0.1.5.9/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 23:27:52.000000 pillar1-0.1.5.9/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:33:58.045808 pillar1-0.1.6/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-20 23:33:58.045688 pillar1-0.1.6/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.6/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:33:58.044903 pillar1-0.1.6/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.6/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3038 2023-06-20 23:33:26.000000 pillar1-0.1.6/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:33:58.045521 pillar1-0.1.6/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-20 23:33:58.000000 pillar1-0.1.6/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 23:33:58.000000 pillar1-0.1.6/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 23:33:58.000000 pillar1-0.1.6/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 23:33:58.000000 pillar1-0.1.6/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 23:33:58.045845 pillar1-0.1.6/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      619 2023-06-20 23:33:54.000000 pillar1-0.1.6/setup.py
```

### Comparing `pillar1-0.1.5.9/PKG-INFO` & `pillar1-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.9
+Version: 0.1.6
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.9/README.md` & `pillar1-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.9/pillar1/pillar1.py` & `pillar1-0.1.6/pillar1/pillar1.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,19 @@
             aws_access_key_id=user_name,
             aws_secret_access_key=password,
             region_name='us-west-2'
         )
 
     def code(self):
         self.cleaned_code = self.response.replace(self.prompt, '').strip()
+        ELS_TO_REMOVE = ['<pre>', '<code>', '</code>', '</pre>']
+        for curr_el_to_remove in ELS_TO_REMOVE:
+            self.cleaned_code = self.cleaned_code.replace(curr_el_to_remove, '')
+
+        self.cleaned_code = self.cleaned_code.replace('\n', '').replace(' ', '')
         print(self.cleaned_code)
 
     def execute(self):
         spark = SparkSession.builder.getOrCreate()
         self.result = spark.sql(self.cleaned_code)
         self.result.show()
```

### Comparing `pillar1-0.1.5.9/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.6/pillar1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.9
+Version: 0.1.6
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.9/setup.py` & `pillar1-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.5.9',
+    version='0.1.6',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

