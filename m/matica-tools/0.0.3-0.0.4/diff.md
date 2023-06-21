# Comparing `tmp/matica_tools-0.0.3.tar.gz` & `tmp/matica_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matica_tools-0.0.3.tar", last modified: Tue Jun 20 22:54:16 2023, max compression
+gzip compressed data, was "matica_tools-0.0.4.tar", last modified: Wed Jun 21 00:21:56 2023, max compression
```

## Comparing `matica_tools-0.0.3.tar` & `matica_tools-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:54:16.353786 matica_tools-0.0.3/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 matica_tools-0.0.3/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 matica_tools-0.0.3/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-20 22:54:16.353621 matica_tools-0.0.3/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      309 2023-06-20 22:27:11.000000 matica_tools-0.0.3/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:54:16.352225 matica_tools-0.0.3/matica_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 22:53:34.000000 matica_tools-0.0.3/matica_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1950 2023-06-20 22:53:34.000000 matica_tools-0.0.3/matica_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     4903 2023-06-20 22:53:34.000000 matica_tools-0.0.3/matica_tools/api.py
--rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-06-19 22:22:57.000000 matica_tools-0.0.3/matica_tools/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:54:16.353393 matica_tools-0.0.3/matica_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      394 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       67 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 22:58:12.000000 matica_tools-0.0.3/matica_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       13 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-20 22:53:51.000000 matica_tools-0.0.3/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-20 22:54:16.353841 matica_tools-0.0.3/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 matica_tools-0.0.3/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 00:21:56.114614 matica_tools-0.0.4/
+-rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 matica_tools-0.0.4/LICENSE
+-rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 matica_tools-0.0.4/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-21 00:21:56.114436 matica_tools-0.0.4/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      309 2023-06-20 22:27:11.000000 matica_tools-0.0.4/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 00:21:56.112614 matica_tools-0.0.4/matica_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 00:15:07.000000 matica_tools-0.0.4/matica_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     2313 2023-06-21 00:15:07.000000 matica_tools-0.0.4/matica_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     9300 2023-06-21 00:15:07.000000 matica_tools-0.0.4/matica_tools/api.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-06-19 22:22:57.000000 matica_tools-0.0.4/matica_tools/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 00:21:56.114148 matica_tools-0.0.4/matica_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      394 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       67 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 22:58:12.000000 matica_tools-0.0.4/matica_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       13 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-21 00:21:35.000000 matica_tools-0.0.4/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-21 00:21:56.114671 matica_tools-0.0.4/setup.cfg
+-rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 matica_tools-0.0.4/setup.py
```

### Comparing `matica_tools-0.0.3/LICENSE` & `matica_tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matica_tools-0.0.3/PKG-INFO` & `matica_tools-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matica_tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/matica_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `matica_tools-0.0.3/matica_tools/_modidx.py` & `matica_tools-0.0.4/matica_tools/_modidx.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/matica_tools',
                 'doc_host': 'https://nakamura196.github.io',
                 'git_url': 'https://github.com/nakamura196/matica_tools',
                 'lib_path': 'matica_tools'},
   'syms': { 'matica_tools.api': { 'matica_tools.api.MaticaAPIClient': ('api.html#maticaapiclient', 'matica_tools/api.py'),
+                                  'matica_tools.api.MaticaAPIClient.__init2__': ( 'api.html#maticaapiclient.__init2__',
+                                                                                  'matica_tools/api.py'),
                                   'matica_tools.api.MaticaAPIClient.__init__': ('api.html#maticaapiclient.__init__', 'matica_tools/api.py'),
                                   'matica_tools.api.MaticaAPIClient.approve_transfer': ( 'api.html#maticaapiclient.approve_transfer',
                                                                                          'matica_tools/api.py'),
                                   'matica_tools.api.MaticaAPIClient.check_transfer_status': ( 'api.html#maticaapiclient.check_transfer_status',
                                                                                               'matica_tools/api.py'),
                                   'matica_tools.api.MaticaAPIClient.get_aip_url': ( 'api.html#maticaapiclient.get_aip_url',
                                                                                     'matica_tools/api.py'),
                                   'matica_tools.api.MaticaAPIClient.ingest': ('api.html#maticaapiclient.ingest', 'matica_tools/api.py'),
                                   'matica_tools.api.MaticaAPIClient.main': ('api.html#maticaapiclient.main', 'matica_tools/api.py'),
+                                  'matica_tools.api.MaticaAPIClient.status': ('api.html#maticaapiclient.status', 'matica_tools/api.py'),
                                   'matica_tools.api.MaticaAPIClient.transfer': ('api.html#maticaapiclient.transfer', 'matica_tools/api.py'),
                                   'matica_tools.api.MaticaAPIClient.upload': ('api.html#maticaapiclient.upload', 'matica_tools/api.py')},
             'matica_tools.core': {'matica_tools.core.foo': ('core.html#foo', 'matica_tools/core.py')}}}
```

### Comparing `matica_tools-0.0.3/matica_tools.egg-info/PKG-INFO` & `matica_tools-0.0.4/matica_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matica-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/matica_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `matica_tools-0.0.3/settings.ini` & `matica_tools-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = matica_tools
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = matica_tools
```

### Comparing `matica_tools-0.0.3/setup.py` & `matica_tools-0.0.4/setup.py`

 * *Files identical despite different names*

