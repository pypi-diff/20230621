# Comparing `tmp/testimony-2.2.0.tar.gz` & `tmp/testimony-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testimony-2.2.0.tar", last modified: Wed Nov 25 04:04:00 2020, max compression
+gzip compressed data, was "testimony-2.3.0.tar", last modified: Wed Jun 21 14:29:31 2023, max compression
```

## Comparing `testimony-2.2.0.tar` & `testimony-2.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 elyezer   (1000) elyezer   (1000)        0 2020-11-25 04:04:00.000000 testimony-2.2.0/
--rwxrwxr-x   0 elyezer   (1000) elyezer   (1000)    35121 2019-05-17 15:17:52.000000 testimony-2.2.0/LICENSE
--rw-rw-r--   0 elyezer   (1000) elyezer   (1000)       35 2019-05-17 15:17:52.000000 testimony-2.2.0/MANIFEST.in
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)     1261 2020-11-25 04:04:00.000000 testimony-2.2.0/PKG-INFO
--rw-rw-r--   0 elyezer   (1000) elyezer   (1000)      469 2019-07-09 15:59:59.000000 testimony-2.2.0/README.rst
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)        6 2020-11-25 04:03:14.000000 testimony-2.2.0/VERSION
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)       38 2020-11-25 04:04:00.000000 testimony-2.2.0/setup.cfg
--rw-rw-r--   0 elyezer   (1000) elyezer   (1000)     1204 2019-07-09 17:39:52.000000 testimony-2.2.0/setup.py
-drwxr-xr-x   0 elyezer   (1000) elyezer   (1000)        0 2020-11-25 04:04:00.000000 testimony-2.2.0/testimony/
--rwxr-xr-x   0 elyezer   (1000) elyezer   (1000)    20591 2020-11-25 04:00:17.000000 testimony-2.2.0/testimony/__init__.py
--rw-rw-r--   0 elyezer   (1000) elyezer   (1000)     1174 2019-05-24 18:13:05.000000 testimony-2.2.0/testimony/cli.py
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)     2536 2020-11-25 04:00:17.000000 testimony-2.2.0/testimony/config.py
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)     1032 2020-11-25 04:00:17.000000 testimony-2.2.0/testimony/constants.py
--rw-rw-r--   0 elyezer   (1000) elyezer   (1000)     5187 2019-05-24 19:05:04.000000 testimony-2.2.0/testimony/parser.py
-drwxr-xr-x   0 elyezer   (1000) elyezer   (1000)        0 2020-11-25 04:04:00.000000 testimony-2.2.0/testimony.egg-info/
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)     1261 2020-11-25 04:04:00.000000 testimony-2.2.0/testimony.egg-info/PKG-INFO
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)      349 2020-11-25 04:04:00.000000 testimony-2.2.0/testimony.egg-info/SOURCES.txt
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)        1 2020-11-25 04:04:00.000000 testimony-2.2.0/testimony.egg-info/dependency_links.txt
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)       73 2020-11-25 04:04:00.000000 testimony-2.2.0/testimony.egg-info/entry_points.txt
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)       32 2020-11-25 04:04:00.000000 testimony-2.2.0/testimony.egg-info/requires.txt
--rw-r--r--   0 elyezer   (1000) elyezer   (1000)       10 2020-11-25 04:04:00.000000 testimony-2.2.0/testimony.egg-info/top_level.txt
+drwxr-xr-x   0 elyezer    (501) staff       (20)        0 2023-06-21 14:29:31.382362 testimony-2.3.0/
+-rwxr-xr-x   0 elyezer    (501) staff       (20)    35121 2023-06-21 13:43:31.000000 testimony-2.3.0/LICENSE
+-rw-r--r--   0 elyezer    (501) staff       (20)       35 2023-06-21 13:43:31.000000 testimony-2.3.0/MANIFEST.in
+-rw-r--r--   0 elyezer    (501) staff       (20)     1089 2023-06-21 14:29:31.382240 testimony-2.3.0/PKG-INFO
+-rw-r--r--   0 elyezer    (501) staff       (20)      469 2023-06-21 13:43:31.000000 testimony-2.3.0/README.rst
+-rw-r--r--   0 elyezer    (501) staff       (20)        6 2023-06-21 14:25:35.000000 testimony-2.3.0/VERSION
+-rw-r--r--   0 elyezer    (501) staff       (20)       38 2023-06-21 14:29:31.382400 testimony-2.3.0/setup.cfg
+-rw-r--r--   0 elyezer    (501) staff       (20)     1155 2023-06-21 14:24:11.000000 testimony-2.3.0/setup.py
+drwxr-xr-x   0 elyezer    (501) staff       (20)        0 2023-06-21 14:29:31.381323 testimony-2.3.0/testimony/
+-rwxr-xr-x   0 elyezer    (501) staff       (20)    20591 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/__init__.py
+-rw-r--r--   0 elyezer    (501) staff       (20)     1174 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/cli.py
+-rw-r--r--   0 elyezer    (501) staff       (20)     2536 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/config.py
+-rw-r--r--   0 elyezer    (501) staff       (20)     1032 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/constants.py
+-rw-r--r--   0 elyezer    (501) staff       (20)     5187 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/parser.py
+drwxr-xr-x   0 elyezer    (501) staff       (20)        0 2023-06-21 14:29:31.382068 testimony-2.3.0/testimony.egg-info/
+-rw-r--r--   0 elyezer    (501) staff       (20)     1089 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/PKG-INFO
+-rw-r--r--   0 elyezer    (501) staff       (20)      349 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/SOURCES.txt
+-rw-r--r--   0 elyezer    (501) staff       (20)        1 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/dependency_links.txt
+-rw-r--r--   0 elyezer    (501) staff       (20)       54 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/entry_points.txt
+-rw-r--r--   0 elyezer    (501) staff       (20)       32 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/requires.txt
+-rw-r--r--   0 elyezer    (501) staff       (20)       10 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `testimony-2.2.0/LICENSE` & `testimony-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testimony-2.2.0/PKG-INFO` & `testimony-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: testimony
-Version: 2.2.0
+Version: 2.3.0
 Summary: Testimony inspects and reports on the python test cases.
 Home-page: https://github.com/SatelliteQE/testimony/
 Author: Suresh Thirugn
 Author-email: sthirugn@redhat.com
-License: UNKNOWN
-Description: Testimony
-        =========
-        
-        Are you tired of managing your test cases in a test case management tool and
-        your test code in a python automation framework?  Testimony can help to use
-        the python automation framework as a test case repository tool.
-        
-        The project testimony is written to inspect and report on the python test
-        cases.  There are several reporting features in this program.
-        
-        The `full documentation <http://testimony-qe.readthedocs.io/>`_ is available on
-        ReadTheDocs.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Testimony
+=========
+
+Are you tired of managing your test cases in a test case management tool and
+your test code in a python automation framework?  Testimony can help to use
+the python automation framework as a test case repository tool.
+
+The project testimony is written to inspect and report on the python test
+cases.  There are several reporting features in this program.
+
+The `full documentation <http://testimony-qe.readthedocs.io/>`_ is available on
+ReadTheDocs.
```

### Comparing `testimony-2.2.0/setup.py` & `testimony-2.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     entry_points="""
         [console_scripts]
         testimony=testimony.cli:testimony
     """,
     description='Testimony inspects and reports on the python test cases.',
```

### Comparing `testimony-2.2.0/testimony/__init__.py` & `testimony-2.3.0/testimony/__init__.py`

 * *Files identical despite different names*

### Comparing `testimony-2.2.0/testimony/cli.py` & `testimony-2.3.0/testimony/cli.py`

 * *Files identical despite different names*

### Comparing `testimony-2.2.0/testimony/config.py` & `testimony-2.3.0/testimony/config.py`

 * *Files identical despite different names*

### Comparing `testimony-2.2.0/testimony/constants.py` & `testimony-2.3.0/testimony/constants.py`

 * *Files identical despite different names*

### Comparing `testimony-2.2.0/testimony/parser.py` & `testimony-2.3.0/testimony/parser.py`

 * *Files identical despite different names*

### Comparing `testimony-2.2.0/testimony.egg-info/PKG-INFO` & `testimony-2.3.0/testimony.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: testimony
-Version: 2.2.0
+Version: 2.3.0
 Summary: Testimony inspects and reports on the python test cases.
 Home-page: https://github.com/SatelliteQE/testimony/
 Author: Suresh Thirugn
 Author-email: sthirugn@redhat.com
-License: UNKNOWN
-Description: Testimony
-        =========
-        
-        Are you tired of managing your test cases in a test case management tool and
-        your test code in a python automation framework?  Testimony can help to use
-        the python automation framework as a test case repository tool.
-        
-        The project testimony is written to inspect and report on the python test
-        cases.  There are several reporting features in this program.
-        
-        The `full documentation <http://testimony-qe.readthedocs.io/>`_ is available on
-        ReadTheDocs.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Testimony
+=========
+
+Are you tired of managing your test cases in a test case management tool and
+your test code in a python automation framework?  Testimony can help to use
+the python automation framework as a test case repository tool.
+
+The project testimony is written to inspect and report on the python test
+cases.  There are several reporting features in this program.
+
+The `full documentation <http://testimony-qe.readthedocs.io/>`_ is available on
+ReadTheDocs.
```

