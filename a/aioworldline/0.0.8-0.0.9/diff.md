# Comparing `tmp/aioworldline-0.0.8.tar.gz` & `tmp/aioworldline-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioworldline-0.0.8.tar", last modified: Wed Jun 21 16:40:30 2023, max compression
+gzip compressed data, was "aioworldline-0.0.9.tar", last modified: Wed Jun 21 16:45:33 2023, max compression
```

## Comparing `aioworldline-0.0.8.tar` & `aioworldline-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.151244 aioworldline-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 16:40:19.000000 aioworldline-0.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.147245 aioworldline-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.147245 aioworldline-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 16:40:19.000000 aioworldline-0.0.8/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-21 16:40:19.000000 aioworldline-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 16:40:19.000000 aioworldline-0.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 16:40:19.000000 aioworldline-0.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-06-21 16:40:19.000000 aioworldline-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-21 16:40:30.151244 aioworldline-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-21 16:40:19.000000 aioworldline-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 16:40:19.000000 aioworldline-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.151244 aioworldline-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-21 16:40:19.000000 aioworldline-0.0.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.151244 aioworldline-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 16:40:19.000000 aioworldline-0.0.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 16:40:19.000000 aioworldline-0.0.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 16:40:19.000000 aioworldline-0.0.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-21 16:40:19.000000 aioworldline-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-21 16:40:19.000000 aioworldline-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 16:40:19.000000 aioworldline-0.0.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 16:40:19.000000 aioworldline-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 16:40:19.000000 aioworldline-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 16:40:19.000000 aioworldline-0.0.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-21 16:40:30.151244 aioworldline-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-21 16:40:19.000000 aioworldline-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.147245 aioworldline-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.151244 aioworldline-0.0.8/src/aioworldline/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-21 16:40:19.000000 aioworldline-0.0.8/src/aioworldline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 16:40:19.000000 aioworldline-0.0.8/src/aioworldline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 16:40:19.000000 aioworldline-0.0.8/src/aioworldline/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-21 16:40:19.000000 aioworldline-0.0.8/src/aioworldline/worldline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.151244 aioworldline-0.0.8/src/aioworldline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-21 16:40:30.000000 aioworldline-0.0.8/src/aioworldline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-21 16:40:30.000000 aioworldline-0.0.8/src/aioworldline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:40:30.000000 aioworldline-0.0.8/src/aioworldline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:40:30.000000 aioworldline-0.0.8/src/aioworldline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 16:40:30.000000 aioworldline-0.0.8/src/aioworldline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 16:40:30.000000 aioworldline-0.0.8/src/aioworldline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:30.151244 aioworldline-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-21 16:40:19.000000 aioworldline-0.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.548901 aioworldline-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 16:45:21.000000 aioworldline-0.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.544901 aioworldline-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.544901 aioworldline-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 16:45:21.000000 aioworldline-0.0.9/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-21 16:45:21.000000 aioworldline-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 16:45:21.000000 aioworldline-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 16:45:21.000000 aioworldline-0.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-06-21 16:45:21.000000 aioworldline-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-21 16:45:33.548901 aioworldline-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-21 16:45:21.000000 aioworldline-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 16:45:21.000000 aioworldline-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.544901 aioworldline-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-21 16:45:21.000000 aioworldline-0.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.544901 aioworldline-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 16:45:21.000000 aioworldline-0.0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 16:45:21.000000 aioworldline-0.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 16:45:21.000000 aioworldline-0.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-21 16:45:21.000000 aioworldline-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-21 16:45:21.000000 aioworldline-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 16:45:21.000000 aioworldline-0.0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 16:45:21.000000 aioworldline-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 16:45:21.000000 aioworldline-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 16:45:21.000000 aioworldline-0.0.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-21 16:45:33.548901 aioworldline-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-21 16:45:21.000000 aioworldline-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.544901 aioworldline-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.544901 aioworldline-0.0.9/src/aioworldline/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-21 16:45:21.000000 aioworldline-0.0.9/src/aioworldline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 16:45:21.000000 aioworldline-0.0.9/src/aioworldline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 16:45:21.000000 aioworldline-0.0.9/src/aioworldline/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-21 16:45:21.000000 aioworldline-0.0.9/src/aioworldline/worldline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.548901 aioworldline-0.0.9/src/aioworldline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-21 16:45:33.000000 aioworldline-0.0.9/src/aioworldline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-21 16:45:33.000000 aioworldline-0.0.9/src/aioworldline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:45:33.000000 aioworldline-0.0.9/src/aioworldline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:45:33.000000 aioworldline-0.0.9/src/aioworldline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 16:45:33.000000 aioworldline-0.0.9/src/aioworldline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 16:45:33.000000 aioworldline-0.0.9/src/aioworldline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:45:33.548901 aioworldline-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-21 16:45:21.000000 aioworldline-0.0.9/tests/conftest.py
```

### Comparing `aioworldline-0.0.8/.coveragerc` & `aioworldline-0.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.8/.github/workflows/python-publish.yaml` & `aioworldline-0.0.9/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.8/.gitignore` & `aioworldline-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.8/LICENSE` & `aioworldline-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.8/PKG-INFO` & `aioworldline-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioworldline
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial Worldline portal data retrieving client
 Home-page: https://github.com/kamikaze/aioworldline
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/aioworldline/wiki
 Platform: any
```

### Comparing `aioworldline-0.0.8/docs/Makefile` & `aioworldline-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.8/docs/conf.py` & `aioworldline-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.8/docs/index.rst` & `aioworldline-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.8/setup.cfg` & `aioworldline-0.0.9/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aioworldline
-version = 0.0.8
+version = 0.0.9
 description = Unofficial Worldline portal data retrieving client
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/aioworldline
```

### Comparing `aioworldline-0.0.8/src/aioworldline/worldline.py` & `aioworldline-0.0.9/src/aioworldline/worldline.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,9 +131,13 @@
     }
 
     async with session.get(EXPORT_LIST_DATA_URL, params=params, allow_redirects=False) as response:
         try:
             return await response.read()
         except ClientOSError as e:
             logger.error(f'Failed reading the response from Worldline: {e}')
+
+            raise
         except Exception as e:
             logger.error(f'Failed reading the response from Worldline: {e}')
+
+            raise
```

### Comparing `aioworldline-0.0.8/src/aioworldline.egg-info/PKG-INFO` & `aioworldline-0.0.9/src/aioworldline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioworldline
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial Worldline portal data retrieving client
 Home-page: https://github.com/kamikaze/aioworldline
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/aioworldline/wiki
 Platform: any
```

### Comparing `aioworldline-0.0.8/src/aioworldline.egg-info/SOURCES.txt` & `aioworldline-0.0.9/src/aioworldline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

