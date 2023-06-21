# Comparing `tmp/prettyc-1.0.6.tar.gz` & `tmp/prettyc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyc-1.0.6.tar", last modified: Wed Jun 21 17:58:13 2023, max compression
+gzip compressed data, was "prettyc-1.0.7.tar", last modified: Wed Jun 21 20:05:43 2023, max compression
```

## Comparing `prettyc-1.0.6.tar` & `prettyc-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-21 17:58:13.260188 prettyc-1.0.6/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.6/LICENSE
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-21 17:58:13.256188 prettyc-1.0.6/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.6/README.md
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-21 17:58:13.256188 prettyc-1.0.6/prettyc.egg-info/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/SOURCES.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/dependency_links.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/entry_points.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-21 17:58:13.000000 prettyc-1.0.6/prettyc.egg-info/top_level.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)   257548 2023-06-21 17:56:59.000000 prettyc-1.0.6/prettyc.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-21 17:58:13.260188 prettyc-1.0.6/setup.cfg
--rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.6/setup.py
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-21 20:05:43.121312 prettyc-1.0.7/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.7/LICENSE
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-21 20:05:43.121312 prettyc-1.0.7/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.7/README.md
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-21 20:05:43.121312 prettyc-1.0.7/prettyc.egg-info/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/SOURCES.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/dependency_links.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/entry_points.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/top_level.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)   257046 2023-06-21 20:04:47.000000 prettyc-1.0.7/prettyc.py
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-21 20:05:43.121312 prettyc-1.0.7/setup.cfg
+-rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.7/setup.py
```

### Comparing `prettyc-1.0.6/LICENSE` & `prettyc-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.6/PKG-INFO` & `prettyc-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.6
+Version: 1.0.7
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.6/README.md` & `prettyc-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.6/prettyc.egg-info/PKG-INFO` & `prettyc-1.0.7/prettyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.6
+Version: 1.0.7
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.6/prettyc.py` & `prettyc-1.0.7/prettyc.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 import sysconfig
 import unicodedata
 import xml.etree.ElementTree
 
 # if empty, use defaults
 _valid_extensions = set([])
 
-__version__ = '1.0.6'
+__version__ = '1.0.7'
 __verbose__ = False
 
 try:
   #  -- pylint: disable=used-before-assignment
   xrange          # Python 2
 except NameError:
   #  -- pylint: disable=redefined-builtin
@@ -135,15 +135,15 @@
       (Category names are printed with the message and look like
       "[whitespace/indent]".)  Filters are evaluated left to right.
       "-FOO" means "do not print categories that start with FOO".
       "+FOO" means "do print categories that start with FOO".
 
       Examples: --filter=-whitespace,+whitespace/braces
                 --filter=-whitespace,-runtime/printf,+runtime/printf_format
-                --filter=-,+build/include_what_you_use
+                --filter=-,+build/include
 
       To see a list of all the categories used in prettyc, pass no arg:
          --filter=
 
     counting=total|toplevel|detailed
       The total number of errors found is always printed. If
       'toplevel' is provided, then the count of errors in each of
@@ -298,15 +298,14 @@
     'build/endif_comment',
     'build/explicit_make_pair',
     'build/forward_decl',
     'build/header_guard',
     'build/include',
     'build/include_alpha',
     'build/include_order',
-    'build/include_what_you_use',
     'build/namespaces_headers',
     'build/namespaces_literals',
     'build/namespaces',
     'build/printf_format',
     'build/storage_class',
     'legal/copyright',
     'readability/alt_tokens',
@@ -6039,22 +6038,14 @@
   # TODO(unknown): Do a better job of finding .h files so we are confident that
   # not having the .h file means there isn't one.
   if not header_found:
     for extension in GetNonHeaderExtensions():
       if filename.endswith('.' + extension):
         return
 
-  # All the lines have been processed, report the errors found.
-  for required_header_unstripped in sorted(required, key=required.__getitem__):
-    template = required[required_header_unstripped][1]
-    if required_header_unstripped.strip('<>"') not in include_dict:
-      error(filename, required[required_header_unstripped][0],
-            'build/include_what_you_use', 4,
-            'Add #include ' + required_header_unstripped + ' for ' + template)
-
 
 _RE_PATTERN_EXPLICIT_MAKEPAIR = re.compile(r'\bmake_pair\s*<')
 
 
 def CheckMakePairUsesDeduction(filename, clean_lines, linenum, error):
   """Check that make_pair's template arguments are deduced.
```

### Comparing `prettyc-1.0.6/setup.py` & `prettyc-1.0.7/setup.py`

 * *Files identical despite different names*

