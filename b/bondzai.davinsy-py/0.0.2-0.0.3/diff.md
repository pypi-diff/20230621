# Comparing `tmp/bondzai.davinsy-py-0.0.2.tar.gz` & `tmp/bondzai.davinsy-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.davinsy-py-0.0.2.tar", last modified: Tue Jun 20 14:30:24 2023, max compression
+gzip compressed data, was "bondzai.davinsy-py-0.0.3.tar", last modified: Wed Jun 21 10:24:23 2023, max compression
```

## Comparing `bondzai.davinsy-py-0.0.2.tar` & `bondzai.davinsy-py-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-20 14:30:24.471500 bondzai.davinsy-py-0.0.2/
--rw-r--r--   0 theo       (501) staff       (20)     9135 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/LICENCE
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      476 2023-06-20 14:30:24.471555 bondzai.davinsy-py-0.0.2/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)       98 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-20 14:30:24.469042 bondzai.davinsy-py-0.0.2/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-20 14:30:24.470558 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/
--rw-r--r--   0 theo       (501) staff       (20)       24 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     3989 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/davinsy.py
--rw-r--r--   0 theo       (501) staff       (20)     5589 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/enums.py
--rw-r--r--   0 theo       (501) staff       (20)      333 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/logger.py
--rw-r--r--   0 theo       (501) staff       (20)    21765 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/model.py
--rw-r--r--   0 theo       (501) staff       (20)    24433 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/operations.py
--rw-r--r--   0 theo       (501) staff       (20)     3342 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/preproc.py
--rw-r--r--   0 theo       (501) staff       (20)     1034 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-20 14:30:24.471396 bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      476 2023-06-20 14:30:24.000000 bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      600 2023-06-20 14:30:24.000000 bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-20 14:30:24.000000 bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-20 14:30:24.000000 bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       26 2023-06-20 14:30:24.000000 bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-06-20 14:30:24.000000 bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-20 14:30:24.000000 bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-06-20 14:29:57.000000 bondzai.davinsy-py-0.0.2/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      580 2023-06-20 14:30:24.471807 bondzai.davinsy-py-0.0.2/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:51:42.056804 bondzai.davinsy-py-0.0.3/
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/NOTICE
+-rwxrwxrwx   0 root         (0) root         (0)      491 2023-06-21 10:51:42.056804 bondzai.davinsy-py-0.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:51:41.541890 bondzai.davinsy-py-0.0.3/bondzai/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:51:41.846032 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/
+-rwxrwxrwx   0 root         (0) root         (0)       24 2023-06-21 10:51:31.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3989 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/davinsy.py
+-rwxrwxrwx   0 root         (0) root         (0)     6243 2023-06-21 10:51:31.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/enums.py
+-rwxrwxrwx   0 root         (0) root         (0)      333 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)    21765 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/model.py
+-rwxrwxrwx   0 root         (0) root         (0)    24433 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/operations.py
+-rwxrwxrwx   0 root         (0) root         (0)     3342 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/preproc.py
+-rwxrwxrwx   0 root         (0) root         (0)     1034 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:51:42.032811 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      491 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      591 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:51:40.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      700 2023-06-21 10:51:42.062380 bondzai.davinsy-py-0.0.3/setup.cfg
```

### Comparing `bondzai.davinsy-py-0.0.2/NOTICE` & `bondzai.davinsy-py-0.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/davinsy.py` & `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/davinsy.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/enums.py` & `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -217,7 +217,32 @@
     OP_PARAM_MATRIX = 0x90001403
     OP_PARAM_EMPTY = 0x90008000
     OP_PARAM_MODE = 0x90008001
     OP_PARAM_REMOVENFIRST = 0x90008003
     OP_PARAM_SHAPE = 0x90008005
 
 
+class KPITypes(Enum):
+    KPI_FREE = 0
+    KPI_TRAINING_TIME_START = 1
+    KPI_TRAINING_TIME_STOP = 2
+    KPI_TRAINING_DATASET_SIZE = 3
+    KPI_TRAINING_NET_SIZE = 4
+    KPI_TRAINING_WM_SIZE = 5
+    KPI_INFER_TIME_START = 6
+    KPI_INFER_TIME_STOP = 7
+    KPI_INFER_WM_SIZE = 8
+    KPI_PREPROC_TIME_START = 9
+    KPI_PREPROC_TIME_STOP = 10
+    KPI_PREPROC_I_TIME_START = 11
+    KPI_PREPROC_I_TIME_STOP = 12
+    KPI_POSTPROC_TIME_START = 13
+    KPI_POSTPROC_TIME_STOP = 14
+    KPI_OTHER_TIME_START = 15
+    KPI_OTHER_TIME_STOP = 16
+    KPI_SIZE_BYTE = 17
+    KPI_SIZE_KBYTE = 18
+    KPI_QI = 19
+    KPI_OTHER_FLOAT = 20
+    KPI_TRAINING_NET_LAYERS = 21
+
+
```

### Comparing `bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/model.py` & `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/model.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/operations.py` & `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/operations.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/preproc.py` & `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/preproc.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.2/bondzai/davinsy_py/utils.py` & `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.2/bondzai.davinsy_py.egg-info/SOURCES.txt` & `bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-LICENCE
 NOTICE
-README.rst
+README.md
 pyproject.toml
 setup.cfg
 ./bondzai/davinsy_py/__init__.py
 ./bondzai/davinsy_py/davinsy.py
 ./bondzai/davinsy_py/enums.py
 ./bondzai/davinsy_py/logger.py
 ./bondzai/davinsy_py/model.py
```

### Comparing `bondzai.davinsy-py-0.0.2/setup.cfg` & `bondzai.davinsy-py-0.0.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 [metadata]
 name = bondzai.davinsy-py
 version = attr: bondzai.davinsy_py.__version__
 author = Bondzai
 description = Bondzai Python API
-long_description = file: README.rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 keywords = davinsy, bondzai
+license = Apache License 2.0
+license_files = 
+	LICENSE
+	NOTICE
 classifiers = 
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: MIT License
+	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	=.
 packages = find_namespace:
 zip_safe = True
```

