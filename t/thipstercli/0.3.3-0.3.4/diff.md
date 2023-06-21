# Comparing `tmp/thipstercli-0.3.3.tar.gz` & `tmp/thipstercli-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.3.3.tar", last modified: Wed Jun 21 07:22:56 2023, max compression
+gzip compressed data, was "thipstercli-0.3.4.tar", last modified: Wed Jun 21 12:53:46 2023, max compression
```

## Comparing `thipstercli-0.3.3.tar` & `thipstercli-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:22:56.434418 thipstercli-0.3.3/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 07:22:52.000000 thipstercli-0.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 07:22:56.434418 thipstercli-0.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-21 07:22:52.000000 thipstercli-0.3.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-21 07:22:52.000000 thipstercli-0.3.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 07:22:56.434418 thipstercli-0.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-21 07:22:53.000000 thipstercli-0.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:22:56.430418 thipstercli-0.3.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 07:22:52.000000 thipstercli-0.3.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 07:22:52.000000 thipstercli-0.3.3/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-21 07:22:52.000000 thipstercli-0.3.3/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     3137 2023-06-21 07:22:52.000000 thipstercli-0.3.3/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-21 07:22:52.000000 thipstercli-0.3.3/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:22:56.430418 thipstercli-0.3.3/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6108 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/cli.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/providers.py
--rw-r--r--   0 root         (0) root         (0)     3438 2023-06-21 07:22:52.000000 thipstercli-0.3.3/thipstercli/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:22:56.434418 thipstercli-0.3.3/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 07:22:56.000000 thipstercli-0.3.3/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-21 07:22:56.000000 thipstercli-0.3.3/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 07:22:56.000000 thipstercli-0.3.3/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-21 07:22:56.000000 thipstercli-0.3.3/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-21 07:22:56.000000 thipstercli-0.3.3/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 07:22:56.000000 thipstercli-0.3.3/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:53:46.815290 thipstercli-0.3.4/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 12:53:43.000000 thipstercli-0.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 12:53:46.815290 thipstercli-0.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-21 12:53:43.000000 thipstercli-0.3.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-21 12:53:43.000000 thipstercli-0.3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 12:53:46.819290 thipstercli-0.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-21 12:53:43.000000 thipstercli-0.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:53:46.815290 thipstercli-0.3.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:53:46.815290 thipstercli-0.3.4/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3438 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:53:46.815290 thipstercli-0.3.4/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.3.3/LICENSE` & `thipstercli-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/PKG-INFO` & `thipstercli-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.3.3
+Version: 0.3.4
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
-Metadata-Version: 2.1 Name: thipstercli Version: 0.3.3 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.3.4 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.3.3/README.md` & `thipstercli-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/pyproject.toml` & `thipstercli-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/setup.py` & `thipstercli-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.3.3/tests/conftest.py` & `thipstercli-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/tests/test_cli.py` & `thipstercli-0.3.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/tests/test_providers.py` & `thipstercli-0.3.4/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/tests/test_repository.py` & `thipstercli-0.3.4/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/thipstercli/cli.py` & `thipstercli-0.3.4/thipstercli/cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/thipstercli/config.py` & `thipstercli-0.3.4/thipstercli/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/thipstercli/display.py` & `thipstercli-0.3.4/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/thipstercli/helpers.py` & `thipstercli-0.3.4/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/thipstercli/providers.py` & `thipstercli-0.3.4/thipstercli/providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/thipstercli/repository.py` & `thipstercli-0.3.4/thipstercli/repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.3/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.3.4/thipstercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.3.3
+Version: 0.3.4
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
-Metadata-Version: 2.1 Name: thipstercli Version: 0.3.3 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.3.4 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.3.3/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.3.4/thipstercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

