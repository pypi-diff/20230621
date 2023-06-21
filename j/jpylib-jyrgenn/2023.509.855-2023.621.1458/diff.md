# Comparing `tmp/jpylib-jyrgenn-2023.509.855.tar.gz` & `tmp/jpylib-jyrgenn-2023.621.1458.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpylib-jyrgenn-2023.509.855.tar", last modified: Tue May  9 06:55:18 2023, max compression
+gzip compressed data, was "jpylib-jyrgenn-2023.621.1458.tar", last modified: Wed Jun 21 12:58:45 2023, max compression
```

## Comparing `jpylib-jyrgenn-2023.509.855.tar` & `jpylib-jyrgenn-2023.621.1458.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ni         (501) staff       (20)        0 2023-05-09 06:55:18.912171 jpylib-jyrgenn-2023.509.855/
--rw-r--r--   0 ni         (501) staff       (20)     1028 2023-05-09 06:55:18.912030 jpylib-jyrgenn-2023.509.855/PKG-INFO
--rw-r--r--   0 ni         (501) staff       (20)      516 2022-03-11 11:18:51.000000 jpylib-jyrgenn-2023.509.855/README.md
-drwxr-xr-x   0 ni         (501) staff       (20)        0 2023-05-09 06:55:18.911237 jpylib-jyrgenn-2023.509.855/jpylib/
--rwxr-xr-x   0 ni         (501) staff       (20)     2577 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/__init__.py
--rwxr-xr-x   0 ni         (501) staff       (20)    12304 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/alerts.py
--rwxr-xr-x   0 ni         (501) staff       (20)     1868 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/assorted.py
--rwxr-xr-x   0 ni         (501) staff       (20)     4537 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/capture.py
--rwxr-xr-x   0 ni         (501) staff       (20)     3329 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/config.py
--rwxr-xr-x   0 ni         (501) staff       (20)      508 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/fntrace.py
--rw-r--r--   0 ni         (501) staff       (20)     4690 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/iohelper.py
--rwxr-xr-x   0 ni         (501) staff       (20)     5860 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/kvs.py
--rw-r--r--   0 ni         (501) staff       (20)     2275 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/multiset.py
--rwxr-xr-x   0 ni         (501) staff       (20)     2720 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/namespace.py
--rw-r--r--   0 ni         (501) staff       (20)     1756 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/numeric.py
--rwxr-xr-x   0 ni         (501) staff       (20)    12320 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/options.py
--rwxr-xr-x   0 ni         (501) staff       (20)     2803 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/process.py
--rwxr-xr-x   0 ni         (501) staff       (20)    10543 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/secrets.py
--rwxr-xr-x   0 ni         (501) staff       (20)     1359 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/sighandler.py
--rw-r--r--   0 ni         (501) staff       (20)      454 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/singleton.py
--rwxr-xr-x   0 ni         (501) staff       (20)     1569 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/stringreader.py
--rwxr-xr-x   0 ni         (501) staff       (20)    10669 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/table.py
--rwxr-xr-x   0 ni         (501) staff       (20)     2988 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/table_templates.py
--rwxr-xr-x   0 ni         (501) staff       (20)     1179 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/terminal.py
--rwxr-xr-x   0 ni         (501) staff       (20)      695 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib/time.py
-drwxr-xr-x   0 ni         (501) staff       (20)        0 2023-05-09 06:55:18.911872 jpylib-jyrgenn-2023.509.855/jpylib_jyrgenn.egg-info/
--rw-r--r--   0 ni         (501) staff       (20)     1028 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib_jyrgenn.egg-info/PKG-INFO
--rw-r--r--   0 ni         (501) staff       (20)      562 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib_jyrgenn.egg-info/SOURCES.txt
--rw-r--r--   0 ni         (501) staff       (20)        1 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib_jyrgenn.egg-info/dependency_links.txt
--rw-r--r--   0 ni         (501) staff       (20)        7 2023-05-09 06:55:18.000000 jpylib-jyrgenn-2023.509.855/jpylib_jyrgenn.egg-info/top_level.txt
--rw-r--r--   0 ni         (501) staff       (20)       38 2023-05-09 06:55:18.912205 jpylib-jyrgenn-2023.509.855/setup.cfg
--rwxr-xr-x   0 ni         (501) staff       (20)     1067 2022-03-11 11:19:38.000000 jpylib-jyrgenn-2023.509.855/setup.py
+drwxr-xr-x   0 ni         (501) staff       (50)        0 2023-06-21 12:58:45.399367 jpylib-jyrgenn-2023.621.1458/
+-rw-r--r--   0 ni         (501) staff       (50)     1068 2023-06-21 12:58:45.399367 jpylib-jyrgenn-2023.621.1458/PKG-INFO
+-rw-r--r--   0 ni         (501) staff       (50)      516 2022-08-12 14:43:01.000000 jpylib-jyrgenn-2023.621.1458/README.md
+drwxr-xr-x   0 ni         (501) staff       (50)        0 2023-06-21 12:58:45.399367 jpylib-jyrgenn-2023.621.1458/jpylib/
+-rwxr-xr-x   0 ni         (501) staff       (50)     2586 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/__init__.py
+-rwxr-xr-x   0 ni         (501) staff       (50)    12304 2023-06-21 12:58:44.000000 jpylib-jyrgenn-2023.621.1458/jpylib/alerts.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     1868 2023-06-21 12:58:44.000000 jpylib-jyrgenn-2023.621.1458/jpylib/assorted.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     4537 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/capture.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     3329 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/config.py
+-rwxr-xr-x   0 ni         (501) staff       (50)      508 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/fntrace.py
+-rw-r--r--   0 ni         (501) staff       (50)     4690 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/iohelper.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     5860 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/kvs.py
+-rw-r--r--   0 ni         (501) staff       (50)     2275 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/multiset.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     2720 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/namespace.py
+-rw-r--r--   0 ni         (501) staff       (50)     1756 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/numeric.py
+-rwxr-xr-x   0 ni         (501) staff       (50)    12320 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/options.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     4286 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/process.py
+-rwxr-xr-x   0 ni         (501) staff       (50)    10543 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/secrets.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     1359 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/sighandler.py
+-rw-r--r--   0 ni         (501) staff       (50)      454 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/singleton.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     1569 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/stringreader.py
+-rwxr-xr-x   0 ni         (501) staff       (50)    10669 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/table.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     2988 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/table_templates.py
+-rwxr-xr-x   0 ni         (501) staff       (50)     1179 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/terminal.py
+-rwxr-xr-x   0 ni         (501) staff       (50)      695 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib/time.py
+drwxr-xr-x   0 ni         (501) staff       (50)        0 2023-06-21 12:58:45.399367 jpylib-jyrgenn-2023.621.1458/jpylib_jyrgenn.egg-info/
+-rw-r--r--   0 ni         (501) staff       (50)     1068 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib_jyrgenn.egg-info/PKG-INFO
+-rw-r--r--   0 ni         (501) staff       (50)      562 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib_jyrgenn.egg-info/SOURCES.txt
+-rw-r--r--   0 ni         (501) staff       (50)        1 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib_jyrgenn.egg-info/dependency_links.txt
+-rw-r--r--   0 ni         (501) staff       (50)        7 2023-06-21 12:58:45.000000 jpylib-jyrgenn-2023.621.1458/jpylib_jyrgenn.egg-info/top_level.txt
+-rw-r--r--   0 ni         (501) staff       (50)       38 2023-06-21 12:58:45.399367 jpylib-jyrgenn-2023.621.1458/setup.cfg
+-rwxr-xr-x   0 ni         (501) staff       (50)     1067 2022-08-12 14:43:01.000000 jpylib-jyrgenn-2023.621.1458/setup.py
```

### Comparing `jpylib-jyrgenn-2023.509.855/PKG-INFO` & `jpylib-jyrgenn-2023.621.1458/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: jpylib-jyrgenn
-Version: 2023.509.855
+Version: 2023.621.1458
 Summary: Utilities library with several more or less independent components
 Home-page: https://git.w21.org/ni/jpylib/
 Author: Juergen Nickelsen
 Author-email: ni@w21.org
-Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2023.509.855/doc/jpylib.md
+License: UNKNOWN
+Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2023.621.1458/doc/jpylib.md
 Project-URL: Source, https://git.w21.org/ni/jpylib/
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Utilities library with several more or less independent components
 
 This library is mainly intended for myself, so I can access it from
 anywhere. But anyone else is welcome to have a look. Documentation
 is still lacking, I know, but that shall change. Testing is better.
 
 The full documentation (what already exists of it) for this version
 is at
-<https://git.w21.org/ni/jpylib/-/blob/v2023.509.855/doc/jpylib.md>
+<https://git.w21.org/ni/jpylib/-/blob/v2023.621.1458/doc/jpylib.md>
 
 [ni@w21.org 2022-03-11]
+
+
```

### Comparing `jpylib-jyrgenn-2023.509.855/README.md` & `jpylib-jyrgenn-2023.621.1458/README.md`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/__init__.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 from .namespace import Namespace
 from .config import Config
 from .secrets import putsecret, getsecret, getsecret_main, putsecret_main, \
      FileModeError
 from .sighandler import sanesighandler
 from .terminal import ttyi, ttyo, ptty
 from .capture import outputCaptured, outputAndExitCaptured, inputFrom
-from .process import backquote
+from .process import backquote, system
 from .assorted import boolish, flatten, is_sequence, identity
 from .numeric import maybe_int, is_int, maybe_num, is_num, \
      avg_midrange, remove_outliers
 from .iohelper import all_input_lines, read_items, read_mapping
 from .time import isotime, isotime_ms, iso_time, iso_time_ms, iso_time_us
 from .table import format_table
 from .singleton import Singleton
 from .multiset import Multiset
 
-version = "2023.509.855"
+version = "2023.621.1458"
 """The version of the `jpylib` package."""
 
 program = os.path.basename(sys.argv[0])
 """The name of the current program without its directory path."""
 
 real_home = pwd.getpwuid(os.getuid()).pw_dir
 """The home directory of the current user as defined for its user id."""
```

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/alerts.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/alerts.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/assorted.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/assorted.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/capture.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/capture.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/config.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/config.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/iohelper.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/iohelper.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/kvs.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/kvs.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/multiset.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/multiset.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/namespace.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/namespace.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/numeric.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/numeric.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/options.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/options.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/secrets.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/secrets.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/sighandler.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/sighandler.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/stringreader.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/stringreader.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/table.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/table.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/table_templates.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/table_templates.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/terminal.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/terminal.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib/time.py` & `jpylib-jyrgenn-2023.621.1458/jpylib/time.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib_jyrgenn.egg-info/PKG-INFO` & `jpylib-jyrgenn-2023.621.1458/jpylib_jyrgenn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: jpylib-jyrgenn
-Version: 2023.509.855
+Version: 2023.621.1458
 Summary: Utilities library with several more or less independent components
 Home-page: https://git.w21.org/ni/jpylib/
 Author: Juergen Nickelsen
 Author-email: ni@w21.org
-Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2023.509.855/doc/jpylib.md
+License: UNKNOWN
+Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2023.621.1458/doc/jpylib.md
 Project-URL: Source, https://git.w21.org/ni/jpylib/
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Utilities library with several more or less independent components
 
 This library is mainly intended for myself, so I can access it from
 anywhere. But anyone else is welcome to have a look. Documentation
 is still lacking, I know, but that shall change. Testing is better.
 
 The full documentation (what already exists of it) for this version
 is at
-<https://git.w21.org/ni/jpylib/-/blob/v2023.509.855/doc/jpylib.md>
+<https://git.w21.org/ni/jpylib/-/blob/v2023.621.1458/doc/jpylib.md>
 
 [ni@w21.org 2022-03-11]
+
+
```

### Comparing `jpylib-jyrgenn-2023.509.855/jpylib_jyrgenn.egg-info/SOURCES.txt` & `jpylib-jyrgenn-2023.621.1458/jpylib_jyrgenn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.509.855/setup.py` & `jpylib-jyrgenn-2023.621.1458/setup.py`

 * *Files identical despite different names*

