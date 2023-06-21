# Comparing `tmp/lb-telemetry-0.0.1.tar.gz` & `tmp/lb-telemetry-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lb-telemetry-0.0.1.tar", last modified: Wed Jun 21 07:17:28 2023, max compression
+gzip compressed data, was "lb-telemetry-0.0.2.tar", last modified: Wed Jun 21 07:23:11 2023, max compression
```

## Comparing `lb-telemetry-0.0.1.tar` & `lb-telemetry-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:17:28.336734 lb-telemetry-0.0.1/
--rw-r--r--   0 cmcclymont   (501) staff       (20)       30 2023-06-09 07:44:16.000000 lb-telemetry-0.0.1/.flake8
--rw-r--r--   0 cmcclymont   (501) staff       (20)       38 2023-06-20 07:46:54.000000 lb-telemetry-0.0.1/.gitignore
--rw-r--r--   0 cmcclymont   (501) staff       (20)     1848 2023-06-19 13:53:10.000000 lb-telemetry-0.0.1/.gitlab-ci.yml
--rw-r--r--   0 cmcclymont   (501) staff       (20)       37 2023-06-09 07:44:16.000000 lb-telemetry-0.0.1/.mypy.ini
--rw-r--r--   0 cmcclymont   (501) staff       (20)      690 2023-06-09 07:44:16.000000 lb-telemetry-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 cmcclymont   (501) staff       (20)    18151 2023-06-09 07:44:16.000000 lb-telemetry-0.0.1/.pylintrc
--rw-r--r--   0 cmcclymont   (501) staff       (20)    35065 2023-06-09 07:44:16.000000 lb-telemetry-0.0.1/LICENSE
--rw-r--r--   0 cmcclymont   (501) staff       (20)     1444 2023-06-21 07:17:28.336861 lb-telemetry-0.0.1/PKG-INFO
--rw-r--r--   0 cmcclymont   (501) staff       (20)      728 2023-06-19 12:43:48.000000 lb-telemetry-0.0.1/README.md
--rw-r--r--   0 cmcclymont   (501) staff       (20)      352 2023-06-21 07:17:23.000000 lb-telemetry-0.0.1/pyproject.toml
--rw-r--r--   0 cmcclymont   (501) staff       (20)      116 2023-06-20 07:41:21.000000 lb-telemetry-0.0.1/requirements.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)      964 2023-06-21 07:17:28.337293 lb-telemetry-0.0.1/setup.cfg
--rw-r--r--   0 cmcclymont   (501) staff       (20)      894 2023-06-09 07:44:16.000000 lb-telemetry-0.0.1/setup.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:17:28.331990 lb-telemetry-0.0.1/src/
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:17:28.335193 lb-telemetry-0.0.1/src/lb_telemetry/
--rw-r--r--   0 cmcclymont   (501) staff       (20)       21 2023-06-20 14:20:00.000000 lb-telemetry-0.0.1/src/lb_telemetry/__init__.py
--rw-r--r--   0 cmcclymont   (501) staff       (20)     3012 2023-06-20 10:02:15.000000 lb-telemetry-0.0.1/src/lb_telemetry/logger.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:17:28.336499 lb-telemetry-0.0.1/src/lb_telemetry/tests/
--rw-r--r--   0 cmcclymont   (501) staff       (20)       60 2023-06-19 12:43:48.000000 lb-telemetry-0.0.1/src/lb_telemetry/tests/__init__.py
--rw-r--r--   0 cmcclymont   (501) staff       (20)     2865 2023-06-21 06:50:03.000000 lb-telemetry-0.0.1/src/lb_telemetry/tests/test_logger.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:17:28.336097 lb-telemetry-0.0.1/src/lb_telemetry.egg-info/
--rw-r--r--   0 cmcclymont   (501) staff       (20)     1444 2023-06-21 07:17:28.000000 lb-telemetry-0.0.1/src/lb_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 cmcclymont   (501) staff       (20)      474 2023-06-21 07:17:28.000000 lb-telemetry-0.0.1/src/lb_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)        1 2023-06-21 07:17:28.000000 lb-telemetry-0.0.1/src/lb_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)       17 2023-06-21 07:17:28.000000 lb-telemetry-0.0.1/src/lb_telemetry.egg-info/requires.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)       13 2023-06-21 07:17:28.000000 lb-telemetry-0.0.1/src/lb_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:23:11.670589 lb-telemetry-0.0.2/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       30 2023-06-09 07:44:16.000000 lb-telemetry-0.0.2/.flake8
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       38 2023-06-20 07:46:54.000000 lb-telemetry-0.0.2/.gitignore
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     1848 2023-06-19 13:53:10.000000 lb-telemetry-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       37 2023-06-09 07:44:16.000000 lb-telemetry-0.0.2/.mypy.ini
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      690 2023-06-09 07:44:16.000000 lb-telemetry-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 cmcclymont   (501) staff       (20)    18151 2023-06-09 07:44:16.000000 lb-telemetry-0.0.2/.pylintrc
+-rw-r--r--   0 cmcclymont   (501) staff       (20)    35065 2023-06-09 07:44:16.000000 lb-telemetry-0.0.2/LICENSE
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     1405 2023-06-21 07:23:11.670685 lb-telemetry-0.0.2/PKG-INFO
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      728 2023-06-19 12:43:48.000000 lb-telemetry-0.0.2/README.md
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      979 2023-06-21 07:22:14.000000 lb-telemetry-0.0.2/pyproject.toml
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      116 2023-06-20 07:41:21.000000 lb-telemetry-0.0.2/requirements.txt
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      250 2023-06-21 07:23:11.671032 lb-telemetry-0.0.2/setup.cfg
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      894 2023-06-09 07:44:16.000000 lb-telemetry-0.0.2/setup.py
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:23:11.665327 lb-telemetry-0.0.2/src/
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:23:11.669027 lb-telemetry-0.0.2/src/lb_telemetry/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       21 2023-06-20 14:20:00.000000 lb-telemetry-0.0.2/src/lb_telemetry/__init__.py
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     3012 2023-06-20 10:02:15.000000 lb-telemetry-0.0.2/src/lb_telemetry/logger.py
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:23:11.670329 lb-telemetry-0.0.2/src/lb_telemetry/tests/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       60 2023-06-19 12:43:48.000000 lb-telemetry-0.0.2/src/lb_telemetry/tests/__init__.py
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     2865 2023-06-21 06:50:03.000000 lb-telemetry-0.0.2/src/lb_telemetry/tests/test_logger.py
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 07:23:11.669888 lb-telemetry-0.0.2/src/lb_telemetry.egg-info/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     1405 2023-06-21 07:23:11.000000 lb-telemetry-0.0.2/src/lb_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      474 2023-06-21 07:23:11.000000 lb-telemetry-0.0.2/src/lb_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 cmcclymont   (501) staff       (20)        1 2023-06-21 07:23:11.000000 lb-telemetry-0.0.2/src/lb_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       17 2023-06-21 07:23:11.000000 lb-telemetry-0.0.2/src/lb_telemetry.egg-info/requires.txt
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       13 2023-06-21 07:23:11.000000 lb-telemetry-0.0.2/src/lb_telemetry.egg-info/top_level.txt
```

### Comparing `lb-telemetry-0.0.1/.gitlab-ci.yml` & `lb-telemetry-0.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.1/.pre-commit-config.yaml` & `lb-telemetry-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.1/.pylintrc` & `lb-telemetry-0.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.1/LICENSE` & `lb-telemetry-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.1/PKG-INFO` & `lb-telemetry-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.0.1
+Version: 0.0.2
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
-Home-page: https://gitlab.cern.ch/lhcb/lb-telemetry
-Author: Cameron McClymont, Daniel Cervenkov, Chris Burr
-Author-email: cameron.duncan.mcclymont@cern.ch, daniel.cervenkov@cern.ch, christopher.burr@cern.ch
-License: GNU General Public License v3 (GPLv3)
+Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
+Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LHCb Package Usage Logger
```

### Comparing `lb-telemetry-0.0.1/README.md` & `lb-telemetry-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.1/setup.py` & `lb-telemetry-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.1/src/lb_telemetry/logger.py` & `lb-telemetry-0.0.2/src/lb_telemetry/logger.py`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.1/src/lb_telemetry/tests/test_logger.py` & `lb-telemetry-0.0.2/src/lb_telemetry/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.1/src/lb_telemetry.egg-info/PKG-INFO` & `lb-telemetry-0.0.2/src/lb_telemetry.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.0.1
+Version: 0.0.2
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
-Home-page: https://gitlab.cern.ch/lhcb/lb-telemetry
-Author: Cameron McClymont, Daniel Cervenkov, Chris Burr
-Author-email: cameron.duncan.mcclymont@cern.ch, daniel.cervenkov@cern.ch, christopher.burr@cern.ch
-License: GNU General Public License v3 (GPLv3)
+Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
+Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LHCb Package Usage Logger
```

