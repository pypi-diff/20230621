# Comparing `tmp/groupeffect-0.2.3.tar.gz` & `tmp/groupeffect-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groupeffect-0.2.3.tar", last modified: Tue Jun 20 20:46:55 2023, max compression
+gzip compressed data, was "groupeffect-0.2.4.tar", last modified: Wed Jun 21 14:16:12 2023, max compression
```

## Comparing `groupeffect-0.2.3.tar` & `groupeffect-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/
--rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.2.3/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3603 2023-06-20 20:46:55.229185 groupeffect-0.2.3/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     2870 2023-06-20 20:45:33.000000 groupeffect-0.2.3/README.md
--rw-rw-r--   0 root         (0) root         (0)      190 2023-06-20 20:46:54.000000 groupeffect-0.2.3/VERSION.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.2.3/groupeffect/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.3/groupeffect/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.3/groupeffect/management/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5529 2023-06-20 20:33:30.000000 groupeffect-0.2.3/groupeffect/management/commands/effect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/management/configuration/
--rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/management/configuration/default.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/management/tasks/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/management/tasks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5510 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/management/tasks/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.225185 groupeffect-0.2.3/groupeffect/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.225185 groupeffect-0.2.3/groupeffect/templates/groupeffect/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/
--rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/database.txt
--rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/serializers.txt
--rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/tests.txt
--rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/urls.txt
--rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/views.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/templates/groupeffect/web/
--rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/web/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3603 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      846 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      821 2023-06-20 20:46:55.233185 groupeffect-0.2.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      417 2023-06-20 20:23:01.000000 groupeffect-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/
+-rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.2.4/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4308 2023-06-21 14:16:12.649204 groupeffect-0.2.4/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     3016 2023-06-21 12:58:29.000000 groupeffect-0.2.4/README.md
+-rw-rw-r--   0 root         (0) root         (0)      190 2023-06-21 14:16:12.000000 groupeffect-0.2.4/VERSION.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.645204 groupeffect-0.2.4/groupeffect/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.2.4/groupeffect/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.4/groupeffect/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.4/groupeffect/management/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5531 2023-06-21 13:14:58.000000 groupeffect-0.2.4/groupeffect/management/commands/effect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/management/configuration/
+-rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/management/configuration/default.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/management/tasks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/management/tasks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5510 2023-06-21 13:10:11.000000 groupeffect-0.2.4/groupeffect/management/tasks/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.645204 groupeffect-0.2.4/groupeffect/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.645204 groupeffect-0.2.4/groupeffect/templates/groupeffect/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/
+-rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/database.txt
+-rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/serializers.txt
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/tests.txt
+-rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/urls.txt
+-rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/views.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/templates/groupeffect/web/
+-rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/web/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.645204 groupeffect-0.2.4/groupeffect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4308 2023-06-21 14:16:12.000000 groupeffect-0.2.4/groupeffect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      812 2023-06-21 14:16:12.000000 groupeffect-0.2.4/groupeffect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 14:16:12.000000 groupeffect-0.2.4/groupeffect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-21 14:16:12.000000 groupeffect-0.2.4/groupeffect.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1269 2023-06-21 14:16:12.649204 groupeffect-0.2.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      417 2023-06-21 13:09:18.000000 groupeffect-0.2.4/setup.py
```

### Comparing `groupeffect-0.2.3/LICENSE` & `groupeffect-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.3/PKG-INFO` & `groupeffect-0.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,62 @@
 Metadata-Version: 2.1
 Name: groupeffect
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Django app for fast api development.
 Home-page: https://github.com/Groupeffect/groupeffect-pypi
 Author: Amir Yousefi
 Author-email: groupeffect.public@gmail.com
 License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GROUPEFFECT-PYPI
+# Groupeffect reusable Django app  
 
 Django app with rest framework integration for fast development.
 Write task classes instead of management commands for faster cli integrations.
 Run enhanced `startapp` command to generate boilerplate `ModelViewSets` from a configuration file.
 
 **Package code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi/tree/main/framework/pypi/app/package
 
 **Development code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi
 
+**PyPi package**
+
+https://pypi.org/project/groupeffect/
+
+**Django package**
+
+https://djangopackages.org/packages/p/groupeffect/
+
 
 # Quick start
 
 1. Add "groupeffect" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [ 
         ...
```

### Comparing `groupeffect-0.2.3/README.md` & `groupeffect-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-# GROUPEFFECT-PYPI
+# Groupeffect reusable Django app  
 
 Django app with rest framework integration for fast development.
 Write task classes instead of management commands for faster cli integrations.
 Run enhanced `startapp` command to generate boilerplate `ModelViewSets` from a configuration file.
 
 **Package code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi/tree/main/framework/pypi/app/package
 
 **Development code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi
 
+**PyPi package**
+
+https://pypi.org/project/groupeffect/
+
+**Django package**
+
+https://djangopackages.org/packages/p/groupeffect/
+
 
 # Quick start
 
 1. Add "groupeffect" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [ 
         ...
```

### Comparing `groupeffect-0.2.3/groupeffect/management/commands/effect.py` & `groupeffect-0.2.4/groupeffect/management/commands/effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import os
 import json
-from django.core.management.base import BaseCommand, CommandParser
+import os
 from django.conf import settings
+from django.core.management.base import BaseCommand, CommandParser
 from django.utils.module_loading import import_string
 
 
 GROUPEFFECT_CLI_OPTIONS = [
     {
         "key": "command",
         "value": "info",
@@ -140,35 +140,34 @@
 
     def read_config_json(self):
         if os.path.exists(self.config_file):
             with open(self.config_file, "r") as f:
                 self.configuration = json.load(f)
         else:
             self.errors.append(
-                f"{self.config_file} does not exists. You can add this file manually if you want. Or add GROUPEFFECT_CONFIG_JSON_FILE_PATH to your settings.py"
+                f"""{self.config_file} does not exists. You can add this file manually if you want.
+Or add GROUPEFFECT_CONFIG_JSON_FILE_PATH to your settings.py"""
             )
 
 
 class Command(BaseCommand):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.success = []
         self.errors = []
         self.configurator = Configurator
         self.cli_options = GROUPEFFECT_CLI_OPTIONS
 
     def add_arguments(self, parser: CommandParser) -> None:
         # https://docs.python.org/3/library/argparse.html#action
-
         for config in self.cli_options:
             if "args" in config and "kwargs" in config:
                 parser.add_argument(*config["args"], **config["kwargs"])
 
     def handle(self, *args, **options) -> str | None:
-
         # Setup configurator
         self.config = self.configurator(options)
 
         # Run tasks
         for i in self.config.tasks:
             task = i(
                 **{
```

### Comparing `groupeffect-0.2.3/groupeffect/management/tasks/default.py` & `groupeffect-0.2.4/groupeffect/management/tasks/default.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
-from django.utils.module_loading import import_string
 import shutil
 from django.conf import settings
 from django.core.management import call_command
 from django.template.loader import get_template
+from django.utils.module_loading import import_string
 
 
 class MetaTask:
     isAbstract = True
 
     def __init__(self, **context) -> None:
         self.GROUPEFFECT_MANAGEMENT_PATH = os.path.abspath(
```

### Comparing `groupeffect-0.2.3/groupeffect/templates/groupeffect/web/api.html` & `groupeffect-0.2.4/groupeffect/templates/groupeffect/web/api.html`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.3/groupeffect.egg-info/PKG-INFO` & `groupeffect-0.2.4/groupeffect.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,62 @@
 Metadata-Version: 2.1
 Name: groupeffect
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Django app for fast api development.
 Home-page: https://github.com/Groupeffect/groupeffect-pypi
 Author: Amir Yousefi
 Author-email: groupeffect.public@gmail.com
 License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GROUPEFFECT-PYPI
+# Groupeffect reusable Django app  
 
 Django app with rest framework integration for fast development.
 Write task classes instead of management commands for faster cli integrations.
 Run enhanced `startapp` command to generate boilerplate `ModelViewSets` from a configuration file.
 
 **Package code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi/tree/main/framework/pypi/app/package
 
 **Development code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi
 
+**PyPi package**
+
+https://pypi.org/project/groupeffect/
+
+**Django package**
+
+https://djangopackages.org/packages/p/groupeffect/
+
 
 # Quick start
 
 1. Add "groupeffect" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [ 
         ...
```

### Comparing `groupeffect-0.2.3/groupeffect.egg-info/SOURCES.txt` & `groupeffect-0.2.4/groupeffect.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.cfg
 setup.py
 groupeffect/__init__.py
 groupeffect/apps.py
 groupeffect.egg-info/PKG-INFO
 groupeffect.egg-info/SOURCES.txt
 groupeffect.egg-info/dependency_links.txt
-groupeffect.egg-info/requires.txt
 groupeffect.egg-info/top_level.txt
 groupeffect/management/__init__.py
 groupeffect/management/commands/__init__.py
 groupeffect/management/commands/effect.py
 groupeffect/management/configuration/default.json
 groupeffect/management/tasks/__init__.py
 groupeffect/management/tasks/default.py
```

