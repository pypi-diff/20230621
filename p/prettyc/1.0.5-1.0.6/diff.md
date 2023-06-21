# Comparing `tmp/prettyc-1.0.5.tar.gz` & `tmp/prettyc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyc-1.0.5.tar", last modified: Fri Jun 16 19:39:20 2023, max compression
+gzip compressed data, was "prettyc-1.0.6.tar", last modified: Wed Jun 21 17:58:13 2023, max compression
```

## Comparing `prettyc-1.0.5.tar` & `prettyc-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-16 19:39:20.145261 prettyc-1.0.5/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.5/LICENSE
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-16 19:39:20.145261 prettyc-1.0.5/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.5/README.md
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-16 19:39:20.145261 prettyc-1.0.5/prettyc.egg-info/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/SOURCES.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/dependency_links.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/entry_points.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/top_level.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)   257930 2023-06-16 19:38:04.000000 prettyc-1.0.5/prettyc.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-16 19:39:20.145261 prettyc-1.0.5/setup.cfg
--rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.5/setup.py
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-21 17:58:13.260188 prettyc-1.0.6/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.6/LICENSE
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-21 17:58:13.256188 prettyc-1.0.6/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.6/README.md
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-21 17:58:13.256188 prettyc-1.0.6/prettyc.egg-info/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/SOURCES.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/dependency_links.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/entry_points.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/top_level.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)   257548 2023-06-21 17:56:59.000000 prettyc-1.0.6/prettyc.py
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-21 17:58:13.260188 prettyc-1.0.6/setup.cfg
+-rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.6/setup.py
```

### Comparing `prettyc-1.0.5/LICENSE` & `prettyc-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.5/PKG-INFO` & `prettyc-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.5/README.md` & `prettyc-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.5/prettyc.egg-info/PKG-INFO` & `prettyc-1.0.6/prettyc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.5/prettyc.py` & `prettyc-1.0.6/prettyc.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 import sysconfig
 import unicodedata
 import xml.etree.ElementTree
 
 # if empty, use defaults
 _valid_extensions = set([])
 
-__version__ = '1.0.5'
+__version__ = '1.0.6'
 __verbose__ = False
 
 try:
   #  -- pylint: disable=used-before-assignment
   xrange          # Python 2
 except NameError:
   #  -- pylint: disable=redefined-builtin
@@ -5389,23 +5389,14 @@
   match = Search(r'snprintf\s*\(([^,]*),\s*([0-9]*)\s*,', line)
   if match and match.group(2) != '0':
     # If 2nd arg is zero, snprintf is used to calculate size.
     error(filename, linenum, 'runtime/printf', 3,
           'If you can, use sizeof(%s) instead of %s as the 2nd arg '
           'to snprintf.' % (match.group(1), match.group(2)))
 
-  # Check if some verboten C functions are being used.
-  if Search(r'\bsprintf\s*\(', line):
-    error(filename, linenum, 'runtime/printf', 5,
-          'Never use sprintf. Use snprintf instead.')
-  match = Search(r'\b(strcpy|strcat)\s*\(', line)
-  if match:
-    error(filename, linenum, 'runtime/printf', 4,
-          'Almost always, snprintf is better than %s' % match.group(1))
-
 
 def IsDerivedFunction(clean_lines, linenum):
   """Check if current line contains an inherited function.
 
   Args:
     clean_lines: A CleansedLines instance containing the file.
     linenum: The number of the line to check.
```

### Comparing `prettyc-1.0.5/setup.py` & `prettyc-1.0.6/setup.py`

 * *Files identical despite different names*

