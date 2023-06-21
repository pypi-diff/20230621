# Comparing `tmp/pythttp-0.1.7.tar.gz` & `tmp/pythttp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.1.7.tar", last modified: Mon Jun 19 15:18:21 2023, max compression
+gzip compressed data, was "pythttp-0.1.8.tar", last modified: Wed Jun 21 10:58:21 2023, max compression
```

## Comparing `pythttp-0.1.7.tar` & `pythttp-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 15:18:21.831640 pythttp-0.1.7/
--rw-rw-rw-   0        0        0     1093 2023-06-19 15:18:21.830637 pythttp-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.7/README.md
--rw-rw-rw-   0        0        0      419 2023-06-19 15:17:28.000000 pythttp-0.1.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-19 15:18:21.823638 pythttp-0.1.7/pythttp/
--rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.7/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     3473 2023-06-19 11:42:45.000000 pythttp-0.1.7/pythttp/Protocol.py
--rw-rw-rw-   0        0        0    18937 2023-06-19 15:16:02.000000 pythttp-0.1.7/pythttp/RequestHandler.py
--rw-rw-rw-   0        0        0     4500 2023-06-19 15:15:22.000000 pythttp-0.1.7/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.7/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.7/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:18:21.829641 pythttp-0.1.7/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 15:18:21.831640 pythttp-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      634 2023-06-19 15:17:30.000000 pythttp-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:58:21.077516 pythttp-0.1.8/
+-rw-rw-rw-   0        0        0     1093 2023-06-21 10:58:21.077516 pythttp-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.8/README.md
+-rw-rw-rw-   0        0        0      419 2023-06-21 10:58:06.000000 pythttp-0.1.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-21 10:58:21.057482 pythttp-0.1.8/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.8/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3473 2023-06-19 11:42:45.000000 pythttp-0.1.8/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0    18937 2023-06-19 15:16:02.000000 pythttp-0.1.8/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     4500 2023-06-19 15:15:22.000000 pythttp-0.1.8/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.8/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.8/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:58:21.075514 pythttp-0.1.8/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-06-21 10:58:20.000000 pythttp-0.1.8/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-21 10:58:20.000000 pythttp-0.1.8/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 10:58:20.000000 pythttp-0.1.8/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-21 10:58:20.000000 pythttp-0.1.8/pythttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 10:58:20.000000 pythttp-0.1.8/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 10:58:21.078515 pythttp-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      634 2023-06-21 10:58:02.000000 pythttp-0.1.8/setup.py
```

### Comparing `pythttp-0.1.7/PKG-INFO` & `pythttp-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.7
+Version: 0.1.8
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.7/README.md` & `pythttp-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.7/pythttp/Log_Manager.py` & `pythttp-0.1.8/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.7/pythttp/Protocol.py` & `pythttp-0.1.8/pythttp/Protocol.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.7/pythttp/RequestHandler.py` & `pythttp-0.1.8/pythttp/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.7/pythttp/Structure.py` & `pythttp-0.1.8/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.7/pythttp/Thread_Manager.py` & `pythttp-0.1.8/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.7/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.8/pythttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.7
+Version: 0.1.8
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.7/setup.py` & `pythttp-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.1.7",
+    version="0.1.8",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=['dataclasses','datetime','uuid'],
```

