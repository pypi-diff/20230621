# Comparing `tmp/assistorg-api-0.0.1.tar.gz` & `tmp/assistorg-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistorg-api-0.0.1.tar", last modified: Wed Jun 21 01:31:43 2023, max compression
+gzip compressed data, was "assistorg-api-0.0.2.tar", last modified: Wed Jun 21 01:40:17 2023, max compression
```

## Comparing `assistorg-api-0.0.1.tar` & `assistorg-api-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 01:31:43.945172 assistorg-api-0.0.1/
--rw-rw-rw-   0        0        0      201 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3835 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       98 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1108 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1676 2023-06-21 01:31:43.945172 assistorg-api-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1043 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-21 01:31:43.929542 assistorg-api-0.0.1/assist_api_wrapper/
--rw-rw-rw-   0        0        0      174 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/assist_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0       20 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/assist_api_wrapper/assist_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:31:43.929542 assistorg-api-0.0.1/assistorg_api.egg-info/
--rw-rw-rw-   0        0        0     1676 2023-06-21 01:31:43.000000 assistorg-api-0.0.1/assistorg_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-06-21 01:31:43.000000 assistorg-api-0.0.1/assistorg_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 01:31:43.000000 assistorg-api-0.0.1/assistorg_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 01:27:29.000000 assistorg-api-0.0.1/assistorg_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-06-21 01:31:43.000000 assistorg-api-0.0.1/assistorg_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 01:31:43.945172 assistorg-api-0.0.1/docs/
--rw-rw-rw-   0        0        0      639 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/authors.rst
--rw-rw-rw-   0        0        0     5128 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/history.rst
--rw-rw-rw-   0        0        0      335 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/index.rst
--rw-rw-rw-   0        0        0     1321 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/installation.rst
--rwxrwxrwx   0        0        0      816 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/readme.rst
--rw-rw-rw-   0        0        0       98 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/docs/usage.rst
--rw-rw-rw-   0        0        0      414 2023-06-21 01:31:43.945172 assistorg-api-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1371 2023-06-21 01:31:39.000000 assistorg-api-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:31:43.945172 assistorg-api-0.0.1/tests/
--rw-rw-rw-   0        0        0       49 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      463 2023-06-19 20:44:40.000000 assistorg-api-0.0.1/tests/test_assist_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.202275 assistorg-api-0.0.2/
+-rw-rw-rw-   0        0        0      201 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3835 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       98 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1108 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1654 2023-06-21 01:40:17.202275 assistorg-api-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1043 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.186645 assistorg-api-0.0.2/assist_api_wrapper/
+-rw-rw-rw-   0        0        0      174 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/assist_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/assist_api_wrapper/assist_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.186645 assistorg-api-0.0.2/assistorg_api.egg-info/
+-rw-rw-rw-   0        0        0     1654 2023-06-21 01:40:17.000000 assistorg-api-0.0.2/assistorg_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-06-21 01:40:17.000000 assistorg-api-0.0.2/assistorg_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 01:40:17.000000 assistorg-api-0.0.2/assistorg_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 01:27:29.000000 assistorg-api-0.0.2/assistorg_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-06-21 01:40:17.000000 assistorg-api-0.0.2/assistorg_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.202275 assistorg-api-0.0.2/docs/
+-rw-rw-rw-   0        0        0      639 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     5128 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/history.rst
+-rw-rw-rw-   0        0        0      335 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1321 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      816 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       98 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/usage.rst
+-rw-rw-rw-   0        0        0      414 2023-06-21 01:40:17.217895 assistorg-api-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2023-06-21 01:39:55.000000 assistorg-api-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.202275 assistorg-api-0.0.2/tests/
+-rw-rw-rw-   0        0        0       49 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/tests/test_assist_api_wrapper.py
```

### Comparing `assistorg-api-0.0.1/CONTRIBUTING.rst` & `assistorg-api-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.1/LICENSE` & `assistorg-api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.1/PKG-INFO` & `assistorg-api-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistorg-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial API wrapper for ASSIST.org's API.
 Home-page: https://github.com/montesclarosglennbenedict/assist_api_wrapper
 Author: Glenn Benedict Montesclaros
 Author-email: montesclarosglennbenedict@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -17,24 +17,24 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # ASSIST API Wrapper
 
-[![image](https://img.shields.io/pypi/v/assist_api_wrapper.svg)](https://pypi.python.org/pypi/assist_api_wrapper)
+[![image](https://img.shields.io/pypi/v/assistorg-api.svg)](https://pypi.python.org/pypi/assistorg-api/)
 
-[![image](https://img.shields.io/travis/montesclarosglennbenedict/assist_api_wrapper.svg)](https://travis-ci.com/montesclarosglennbenedict/assist_api_wrapper)
+[![image](https://img.shields.io/travis/montesclarosglennbenedict/assistorg-api.svg)](https://travis-ci.com/montesclarosglennbenedict/assistorg-api)
 
-[![Documentation Status](https://readthedocs.org/projects/assist-api-wrapper/badge/?version=latest)](https://assist-api-wrapper.readthedocs.io/en/latest/?version=latest)
+[![Documentation Status](https://readthedocs.org/projects/assistorg-api/badge/?version=latest)](https://assistorg-api.readthedocs.io/en/latest/?version=latest)
 
-Unofficial API wrapper for ASSIST.org\'s API.
+Unofficial API wrapper for ASSIST.org\'s API. UNRELEASED.
 
 -   Free software: MIT license
--   Documentation: <https://assist-api-wrapper.readthedocs.io>.
+-   Documentation: <https://assistorg-api.readthedocs.io>.
 
 ## Features
 
 -   TODO
 
 ## Credits
```

### Comparing `assistorg-api-0.0.1/README.rst` & `assistorg-api-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.1/assistorg_api.egg-info/PKG-INFO` & `assistorg-api-0.0.2/assistorg_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistorg-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial API wrapper for ASSIST.org's API.
 Home-page: https://github.com/montesclarosglennbenedict/assist_api_wrapper
 Author: Glenn Benedict Montesclaros
 Author-email: montesclarosglennbenedict@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -17,24 +17,24 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # ASSIST API Wrapper
 
-[![image](https://img.shields.io/pypi/v/assist_api_wrapper.svg)](https://pypi.python.org/pypi/assist_api_wrapper)
+[![image](https://img.shields.io/pypi/v/assistorg-api.svg)](https://pypi.python.org/pypi/assistorg-api/)
 
-[![image](https://img.shields.io/travis/montesclarosglennbenedict/assist_api_wrapper.svg)](https://travis-ci.com/montesclarosglennbenedict/assist_api_wrapper)
+[![image](https://img.shields.io/travis/montesclarosglennbenedict/assistorg-api.svg)](https://travis-ci.com/montesclarosglennbenedict/assistorg-api)
 
-[![Documentation Status](https://readthedocs.org/projects/assist-api-wrapper/badge/?version=latest)](https://assist-api-wrapper.readthedocs.io/en/latest/?version=latest)
+[![Documentation Status](https://readthedocs.org/projects/assistorg-api/badge/?version=latest)](https://assistorg-api.readthedocs.io/en/latest/?version=latest)
 
-Unofficial API wrapper for ASSIST.org\'s API.
+Unofficial API wrapper for ASSIST.org\'s API. UNRELEASED.
 
 -   Free software: MIT license
--   Documentation: <https://assist-api-wrapper.readthedocs.io>.
+-   Documentation: <https://assistorg-api.readthedocs.io>.
 
 ## Features
 
 -   TODO
 
 ## Credits
```

### Comparing `assistorg-api-0.0.1/assistorg_api.egg-info/SOURCES.txt` & `assistorg-api-0.0.2/assistorg_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.1/docs/Makefile` & `assistorg-api-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.1/docs/conf.py` & `assistorg-api-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.1/docs/installation.rst` & `assistorg-api-0.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.1/docs/make.bat` & `assistorg-api-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.1/setup.py` & `assistorg-api-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 requirements = []
 
 test_requirements = []
 
 setup(
     name='assistorg-api',
-    version='0.0.1',
+    version='0.0.2',
     description="Unofficial API wrapper for ASSIST.org's API.",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author="Glenn Benedict Montesclaros",
     author_email='montesclarosglennbenedict@gmail.com',
     url='https://github.com/montesclarosglennbenedict/assist_api_wrapper',
     packages=find_packages(include=['assist_api_wrapper', 'assist_api_wrapper.*']),
```

