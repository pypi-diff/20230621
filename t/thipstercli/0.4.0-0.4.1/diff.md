# Comparing `tmp/thipstercli-0.4.0.tar.gz` & `tmp/thipstercli-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.4.0.tar", last modified: Wed Jun 21 13:13:20 2023, max compression
+gzip compressed data, was "thipstercli-0.4.1.tar", last modified: Wed Jun 21 14:28:57 2023, max compression
```

## Comparing `thipstercli-0.4.0.tar` & `thipstercli-0.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.122813 thipstercli-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 13:13:16.000000 thipstercli-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 13:13:20.122813 thipstercli-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-21 13:13:16.000000 thipstercli-0.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-21 13:13:16.000000 thipstercli-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:13:20.122813 thipstercli-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-21 13:13:16.000000 thipstercli-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.118812 thipstercli-0.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.118812 thipstercli-0.4.0/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6293 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.122813 thipstercli-0.4.0/thipstercli/commands/
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8194 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/commands/info.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/commands/providers.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/commands/repository.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.122813 thipstercli-0.4.0/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      284 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:28:57.216812 thipstercli-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 14:28:54.000000 thipstercli-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 14:28:57.216812 thipstercli-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-21 14:28:54.000000 thipstercli-0.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-21 14:28:54.000000 thipstercli-0.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 14:28:57.216812 thipstercli-0.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-21 14:28:54.000000 thipstercli-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:28:57.212812 thipstercli-0.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 14:28:54.000000 thipstercli-0.4.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 14:28:54.000000 thipstercli-0.4.1/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-21 14:28:54.000000 thipstercli-0.4.1/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-21 14:28:54.000000 thipstercli-0.4.1/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-21 14:28:54.000000 thipstercli-0.4.1/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-21 14:28:54.000000 thipstercli-0.4.1/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:28:57.212812 thipstercli-0.4.1/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6293 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:28:57.216812 thipstercli-0.4.1/thipstercli/commands/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8194 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/commands/info.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/commands/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/commands/repository.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-21 14:28:54.000000 thipstercli-0.4.1/thipstercli/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:28:57.212812 thipstercli-0.4.1/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 14:28:57.000000 thipstercli-0.4.1/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-21 14:28:57.000000 thipstercli-0.4.1/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 14:28:57.000000 thipstercli-0.4.1/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-21 14:28:57.000000 thipstercli-0.4.1/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-21 14:28:57.000000 thipstercli-0.4.1/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 14:28:57.000000 thipstercli-0.4.1/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.4.0/LICENSE` & `thipstercli-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/PKG-INFO` & `thipstercli-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.4.0
+Version: 0.4.1
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.4.0 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.4.1 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.4.0/README.md` & `thipstercli-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/pyproject.toml` & `thipstercli-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/setup.py` & `thipstercli-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.4.0/tests/conftest.py` & `thipstercli-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/tests/test_cli.py` & `thipstercli-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/tests/test_info.py` & `thipstercli-0.4.1/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/tests/test_providers.py` & `thipstercli-0.4.1/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/tests/test_repository.py` & `thipstercli-0.4.1/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/thipstercli/cli.py` & `thipstercli-0.4.1/thipstercli/cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/thipstercli/commands/info.py` & `thipstercli-0.4.1/thipstercli/commands/info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/thipstercli/commands/providers.py` & `thipstercli-0.4.1/thipstercli/commands/providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/thipstercli/commands/repository.py` & `thipstercli-0.4.1/thipstercli/commands/repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/thipstercli/config.py` & `thipstercli-0.4.1/thipstercli/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/thipstercli/display.py` & `thipstercli-0.4.1/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/thipstercli/helpers.py` & `thipstercli-0.4.1/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.0/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.4.1/thipstercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.4.0
+Version: 0.4.1
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.4.0 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.4.1 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.4.0/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.4.1/thipstercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

