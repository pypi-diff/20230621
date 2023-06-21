# Comparing `tmp/semremover-0.0.3.tar.gz` & `tmp/semremover-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semremover-0.0.3.tar", last modified: Tue Jun 20 20:28:19 2023, max compression
+gzip compressed data, was "semremover-0.0.4.tar", last modified: Wed Jun 21 06:07:43 2023, max compression
```

## Comparing `semremover-0.0.3.tar` & `semremover-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:28:19.409792 semremover-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 20:27:53.000000 semremover-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-20 20:28:19.409792 semremover-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-20 20:27:53.000000 semremover-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-20 20:28:10.000000 semremover-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:28:19.409792 semremover-0.0.3/semremover/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 20:27:53.000000 semremover-0.0.3/semremover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-20 20:27:53.000000 semremover-0.0.3/semremover/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:28:19.409792 semremover-0.0.3/semremover/models/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 20:27:53.000000 semremover-0.0.3/semremover/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-20 20:27:53.000000 semremover-0.0.3/semremover/models/lama.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-20 20:27:53.000000 semremover-0.0.3/semremover/models/maskformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-20 20:27:53.000000 semremover-0.0.3/semremover/models/semremover.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-20 20:27:53.000000 semremover-0.0.3/semremover/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:28:19.409792 semremover-0.0.3/semremover.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-20 20:28:19.000000 semremover-0.0.3/semremover.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 20:28:19.000000 semremover-0.0.3/semremover.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:28:19.000000 semremover-0.0.3/semremover.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 20:28:19.000000 semremover-0.0.3/semremover.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 20:28:19.413792 semremover-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 20:27:53.000000 semremover-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:07:43.439881 semremover-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 06:07:39.000000 semremover-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-21 06:07:43.439881 semremover-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-21 06:07:39.000000 semremover-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-21 06:07:41.000000 semremover-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:07:43.435881 semremover-0.0.4/semremover/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:07:43.435881 semremover-0.0.4/semremover/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/lama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/maskformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/semremover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:07:43.435881 semremover-0.0.4/semremover.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-21 06:07:43.000000 semremover-0.0.4/semremover.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 06:07:43.000000 semremover-0.0.4/semremover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:07:43.000000 semremover-0.0.4/semremover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 06:07:43.000000 semremover-0.0.4/semremover.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 06:07:43.439881 semremover-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 06:07:39.000000 semremover-0.0.4/setup.py
```

### Comparing `semremover-0.0.3/LICENSE` & `semremover-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `semremover-0.0.3/PKG-INFO` & `semremover-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semremover
-Version: 0.0.3
+Version: 0.0.4
 Summary: semantic object removal made easy.
 Author-email: Jesse Visser <jssvssr2000@gmail.com>
 Project-URL: Homepage, https://github.com/Jessseee/semantic-object-removal
 Project-URL: Bug Tracker, https://github.com/Jessseee/semantic-object-removal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,16 @@
 Install the package.
 ```
 python -m pip install semremover
 ```
 
 Use the `SemanticObjectRemover` in your code.
 ``` python
+from semremover import SemanticObjectRemover
+
 sem_obj_remover = SemanticObjectRemover()
 labels = ['car', 'minibike', 'van']
 inpainted_image = sem_obj_remover.remove_objects_from_image("example.jpg", labels)
 ```
 
 ## Development
```

### Comparing `semremover-0.0.3/README.md` & `semremover-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 Install the package.
 ```
 python -m pip install semremover
 ```
 
 Use the `SemanticObjectRemover` in your code.
 ``` python
+from semremover import SemanticObjectRemover
+
 sem_obj_remover = SemanticObjectRemover()
 labels = ['car', 'minibike', 'van']
 inpainted_image = sem_obj_remover.remove_objects_from_image("example.jpg", labels)
 ```
 
 ## Development
```

### Comparing `semremover-0.0.3/pyproject.toml` & `semremover-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semremover"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jesse Visser", email="jssvssr2000@gmail.com" },
 ]
 description = "semantic object removal made easy."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `semremover-0.0.3/semremover/__main__.py` & `semremover-0.0.4/semremover/__main__.py`

 * *Files identical despite different names*

### Comparing `semremover-0.0.3/semremover/models/lama.py` & `semremover-0.0.4/semremover/models/lama.py`

 * *Files identical despite different names*

### Comparing `semremover-0.0.3/semremover/models/maskformer.py` & `semremover-0.0.4/semremover/models/maskformer.py`

 * *Files identical despite different names*

### Comparing `semremover-0.0.3/semremover/models/semremover.py` & `semremover-0.0.4/semremover/models/semremover.py`

 * *Files identical despite different names*

### Comparing `semremover-0.0.3/semremover.egg-info/PKG-INFO` & `semremover-0.0.4/semremover.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semremover
-Version: 0.0.3
+Version: 0.0.4
 Summary: semantic object removal made easy.
 Author-email: Jesse Visser <jssvssr2000@gmail.com>
 Project-URL: Homepage, https://github.com/Jessseee/semantic-object-removal
 Project-URL: Bug Tracker, https://github.com/Jessseee/semantic-object-removal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,16 @@
 Install the package.
 ```
 python -m pip install semremover
 ```
 
 Use the `SemanticObjectRemover` in your code.
 ``` python
+from semremover import SemanticObjectRemover
+
 sem_obj_remover = SemanticObjectRemover()
 labels = ['car', 'minibike', 'van']
 inpainted_image = sem_obj_remover.remove_objects_from_image("example.jpg", labels)
 ```
 
 ## Development
```

