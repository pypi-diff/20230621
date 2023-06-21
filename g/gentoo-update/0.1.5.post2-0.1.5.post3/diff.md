# Comparing `tmp/gentoo-update-0.1.5.post2.tar.gz` & `tmp/gentoo-update-0.1.5.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo-update-0.1.5.post2.tar", last modified: Tue Jun 20 20:35:13 2023, max compression
+gzip compressed data, was "gentoo-update-0.1.5.post3.tar", last modified: Tue Jun 20 21:05:29 2023, max compression
```

## Comparing `gentoo-update-0.1.5.post2.tar` & `gentoo-update-0.1.5.post3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:35:13.922188 gentoo-update-0.1.5.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-20 20:35:13.922188 gentoo-update-0.1.5.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:35:13.922188 gentoo-update-0.1.5.post2/gentoo_update/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/gentoo_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/gentoo_update/gentoo_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:35:13.922188 gentoo-update-0.1.5.post2/gentoo_update/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4792 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/gentoo_update/scripts/updater.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/gentoo_update/shell_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:35:13.922188 gentoo-update-0.1.5.post2/gentoo_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-20 20:35:13.000000 gentoo-update-0.1.5.post2/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 20:35:13.000000 gentoo-update-0.1.5.post2/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:35:13.000000 gentoo-update-0.1.5.post2/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 20:35:13.000000 gentoo-update-0.1.5.post2/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 20:35:13.000000 gentoo-update-0.1.5.post2/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-20 20:35:13.926188 gentoo-update-0.1.5.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:35:13.922188 gentoo-update-0.1.5.post2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-20 20:34:59.000000 gentoo-update-0.1.5.post2/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:29.988573 gentoo-update-0.1.5.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-20 21:05:29.988573 gentoo-update-0.1.5.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:29.988573 gentoo-update-0.1.5.post3/gentoo_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/gentoo_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/gentoo_update/gentoo_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:29.988573 gentoo-update-0.1.5.post3/gentoo_update/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4792 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/gentoo_update/scripts/updater.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/gentoo_update/shell_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:29.988573 gentoo-update-0.1.5.post3/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-20 21:05:29.000000 gentoo-update-0.1.5.post3/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 21:05:29.000000 gentoo-update-0.1.5.post3/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:05:29.000000 gentoo-update-0.1.5.post3/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 21:05:29.000000 gentoo-update-0.1.5.post3/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 21:05:29.000000 gentoo-update-0.1.5.post3/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-20 21:05:29.988573 gentoo-update-0.1.5.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:29.988573 gentoo-update-0.1.5.post3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-20 21:05:16.000000 gentoo-update-0.1.5.post3/tests/test_updater.py
```

### Comparing `gentoo-update-0.1.5.post2/LICENSE` & `gentoo-update-0.1.5.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.5.post2/PKG-INFO` & `gentoo-update-0.1.5.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.5.post2
+Version: 0.1.5.post3
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gentoo-update-0.1.5.post2/README.md` & `gentoo-update-0.1.5.post3/README.md`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.5.post2/gentoo_update/gentoo_update.py` & `gentoo-update-0.1.5.post3/gentoo_update/gentoo_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import argparse
 from .shell_runner import ShellRunner
 from typing import List
 
-__version__ = "0.1.5-2"
+__version__ = "0.1.5-3"
 current_path = os.path.dirname(os.path.realpath(__file__))
 
 
 def create_cli() -> argparse.Namespace:
     """
     Define CLI command flags using argparse.
```

### Comparing `gentoo-update-0.1.5.post2/gentoo_update/scripts/updater.sh` & `gentoo-update-0.1.5.post3/gentoo_update/scripts/updater.sh`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.5.post2/gentoo_update/shell_runner.py` & `gentoo-update-0.1.5.post3/gentoo_update/shell_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import sys
 import shlex
 import logging
 import subprocess
+from pkg_resources import resource_filename
 from configparser import ConfigParser
 from datetime import datetime
 from typing import Tuple, List
 
 
 class ShellRunner:
     def __init__(self, quiet: str) -> None:
@@ -14,16 +15,15 @@
 
         self.timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M")
         self.make_conf = self.make_conf_reader()
         self.log_dir, self.log_dir_messages = self.initiate_log_directory()
         self.log_filename = f"{self.log_dir}/log_{self.timestamp}"
         self.logger = self.initiate_logger()
 
-        self.script_dir = os.path.join(os.path.dirname(__file__), "scripts")
-        self.script_path = os.path.join(self.script_dir, "updater.sh")
+        self.script_path = resource_filename("gentoo_update", "scripts/updater.sh")
 
     def make_conf_reader(self) -> ConfigParser:
         """
         Read /etc/portage/make.conf with configparser.
 
         Returns:
             configparser.ConfigParser: ConfigParser object.
```

### Comparing `gentoo-update-0.1.5.post2/gentoo_update.egg-info/PKG-INFO` & `gentoo-update-0.1.5.post3/gentoo_update.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.5.post2
+Version: 0.1.5.post3
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gentoo-update-0.1.5.post2/setup.cfg` & `gentoo-update-0.1.5.post3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.10
 	Operating System :: POSIX :: Linux
 
 [options]
 python_requires = >=3.10
+packages = gentoo_update
 include_package_data = True
-packages = 
-	gentoo_update
-	gentoo_update.scripts
+
+[data_files]
+gentoo_update_data = gentoo_update/scripts/updater.sh
 
 [options.entry_points]
 console_scripts = 
 	gentoo-update = gentoo_update.gentoo_update:main
 
 [egg_info]
 tag_build =
```

### Comparing `gentoo-update-0.1.5.post2/tests/test_updater.py` & `gentoo-update-0.1.5.post3/tests/test_updater.py`

 * *Files identical despite different names*

