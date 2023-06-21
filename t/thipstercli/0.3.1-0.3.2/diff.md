# Comparing `tmp/thipstercli-0.3.1.tar.gz` & `tmp/thipstercli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.3.1.tar", last modified: Fri Jun 16 12:09:36 2023, max compression
+gzip compressed data, was "thipstercli-0.3.2.tar", last modified: Wed Jun 21 07:09:21 2023, max compression
```

## Comparing `thipstercli-0.3.1.tar` & `thipstercli-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:09:36.107291 thipstercli-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 12:09:32.000000 thipstercli-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 12:09:36.107291 thipstercli-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-16 12:09:32.000000 thipstercli-0.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-16 12:09:32.000000 thipstercli-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:09:36.107291 thipstercli-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-16 12:09:33.000000 thipstercli-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:09:36.107291 thipstercli-0.3.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     3137 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:09:36.107291 thipstercli-0.3.1/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6108 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/cli.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/providers.py
--rw-r--r--   0 root         (0) root         (0)     3438 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:09:36.107291 thipstercli-0.3.1/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:09:21.716479 thipstercli-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 07:09:17.000000 thipstercli-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 07:09:21.716479 thipstercli-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-21 07:09:17.000000 thipstercli-0.3.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-21 07:09:17.000000 thipstercli-0.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 07:09:21.716479 thipstercli-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-21 07:09:18.000000 thipstercli-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:09:21.712479 thipstercli-0.3.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 07:09:17.000000 thipstercli-0.3.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 07:09:17.000000 thipstercli-0.3.2/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-21 07:09:17.000000 thipstercli-0.3.2/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-21 07:09:17.000000 thipstercli-0.3.2/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-21 07:09:17.000000 thipstercli-0.3.2/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:09:21.716479 thipstercli-0.3.2/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3438 2023-06-21 07:09:17.000000 thipstercli-0.3.2/thipstercli/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:09:21.716479 thipstercli-0.3.2/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 07:09:21.000000 thipstercli-0.3.2/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-21 07:09:21.000000 thipstercli-0.3.2/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 07:09:21.000000 thipstercli-0.3.2/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-21 07:09:21.000000 thipstercli-0.3.2/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-21 07:09:21.000000 thipstercli-0.3.2/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 07:09:21.000000 thipstercli-0.3.2/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.3.1/LICENSE` & `thipstercli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/PKG-INFO` & `thipstercli-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.3.1
+Version: 0.3.2
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
-Metadata-Version: 2.1 Name: thipstercli Version: 0.3.1 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.3.2 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.3.1/README.md` & `thipstercli-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/pyproject.toml` & `thipstercli-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/setup.py` & `thipstercli-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.3.1/tests/conftest.py` & `thipstercli-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/tests/test_cli.py` & `thipstercli-0.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/tests/test_providers.py` & `thipstercli-0.3.2/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/tests/test_repository.py` & `thipstercli-0.3.2/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/thipstercli/cli.py` & `thipstercli-0.3.2/thipstercli/cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/thipstercli/config.py` & `thipstercli-0.3.2/thipstercli/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/thipstercli/display.py` & `thipstercli-0.3.2/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/thipstercli/helpers.py` & `thipstercli-0.3.2/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/thipstercli/providers.py` & `thipstercli-0.3.2/thipstercli/providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/thipstercli/repository.py` & `thipstercli-0.3.2/thipstercli/repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.1/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.3.2/thipstercli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.3.1
+Version: 0.3.2
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
-Metadata-Version: 2.1 Name: thipstercli Version: 0.3.1 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.3.2 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.3.1/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.3.2/thipstercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

