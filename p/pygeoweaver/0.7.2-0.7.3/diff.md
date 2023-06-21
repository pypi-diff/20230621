# Comparing `tmp/pygeoweaver-0.7.2.tar.gz` & `tmp/pygeoweaver-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.7.2.tar", last modified: Wed Jun 21 05:38:30 2023, max compression
+gzip compressed data, was "pygeoweaver-0.7.3.tar", last modified: Wed Jun 21 06:15:19 2023, max compression
```

## Comparing `pygeoweaver-0.7.2.tar` & `pygeoweaver-0.7.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:30.233150 pygeoweaver-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 05:38:30.233150 pygeoweaver-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:30.229150 pygeoweaver-0.7.2/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/download_gw.bat
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/download_gw.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/java_bin.bat
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/java_bin.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/jdk_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_find.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_resetpassword.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/start.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/start.sh
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/stop.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:30.229150 pygeoweaver-0.7.2/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 05:38:30.000000 pygeoweaver-0.7.2/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 05:38:30.000000 pygeoweaver-0.7.2/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:38:30.000000 pygeoweaver-0.7.2/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 05:38:30.000000 pygeoweaver-0.7.2/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 05:38:30.233150 pygeoweaver-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:30.233150 pygeoweaver-0.7.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/test/test_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:15:19.241109 pygeoweaver-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 06:15:19.241109 pygeoweaver-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:15:19.241109 pygeoweaver-0.7.3/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/download_gw.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/download_gw.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/java_bin.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/java_bin.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/jdk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/sc_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/start.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/stop.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:15:19.241109 pygeoweaver-0.7.3/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 06:15:19.000000 pygeoweaver-0.7.3/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-21 06:15:19.000000 pygeoweaver-0.7.3/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:15:19.000000 pygeoweaver-0.7.3/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 06:15:19.000000 pygeoweaver-0.7.3/pygeoweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 06:15:19.000000 pygeoweaver-0.7.3/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 06:15:19.241109 pygeoweaver-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:15:19.241109 pygeoweaver-0.7.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/test/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-21 06:15:06.000000 pygeoweaver-0.7.3/test/test_server.py
```

### Comparing `pygeoweaver-0.7.2/LICENSE` & `pygeoweaver-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/PKG-INFO` & `pygeoweaver-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.7.2
+Version: 0.7.3
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <4,>=3.7
```

### Comparing `pygeoweaver-0.7.2/README.md` & `pygeoweaver-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/__main__.py` & `pygeoweaver-0.7.3/pygeoweaver/__main__.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/jdk_utils.py` & `pygeoweaver-0.7.3/pygeoweaver/jdk_utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_create.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_create.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_detail.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_export.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_find.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_find.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_help.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_help.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_history.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_history.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_import.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_list.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_resetpassword.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_resetpassword.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_run.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_run.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/sc_sync.py` & `pygeoweaver-0.7.3/pygeoweaver/sc_sync.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/server.py` & `pygeoweaver-0.7.3/pygeoweaver/server.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/start.bat` & `pygeoweaver-0.7.3/pygeoweaver/start.bat`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/start.sh` & `pygeoweaver-0.7.3/pygeoweaver/start.sh`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver/utils.py` & `pygeoweaver-0.7.3/pygeoweaver/utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.7.3/pygeoweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.7.2
+Version: 0.7.3
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <4,>=3.7
```

### Comparing `pygeoweaver-0.7.2/pygeoweaver.egg-info/SOURCES.txt` & `pygeoweaver-0.7.3/pygeoweaver.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,11 +27,12 @@
 pygeoweaver/start.sh
 pygeoweaver/stop.bat
 pygeoweaver/stop.sh
 pygeoweaver/utils.py
 pygeoweaver.egg-info/PKG-INFO
 pygeoweaver.egg-info/SOURCES.txt
 pygeoweaver.egg-info/dependency_links.txt
+pygeoweaver.egg-info/requires.txt
 pygeoweaver.egg-info/top_level.txt
 test/__init__.py
 test/test_detail.py
 test/test_server.py
```

### Comparing `pygeoweaver-0.7.2/pyproject.toml` & `pygeoweaver-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "pytest-cov"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7,<4"
 classifiers = [
@@ -18,23 +18,24 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.7.2"
+version = "0.7.3"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
 setuptools = ">=61.0"
 requests = "2.28.2"
 pydantic = "1.10.9"
 
 [tool.poetry.scripts]
 
 [tool.pytest.ini_options]
-addopts = "-p no:warnings --cov=pygeoweaver --cov-report=html"
+addopts = "-p no:warnings --cov=pygeoweaver --cov-report=html"
+
```

### Comparing `pygeoweaver-0.7.2/test/test_detail.py` & `pygeoweaver-0.7.3/test/test_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.2/test/test_server.py` & `pygeoweaver-0.7.3/test/test_server.py`

 * *Files identical despite different names*

