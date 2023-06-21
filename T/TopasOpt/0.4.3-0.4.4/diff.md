# Comparing `tmp/TopasOpt-0.4.3.tar.gz` & `tmp/TopasOpt-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TopasOpt-0.4.3.tar", last modified: Tue Jun  6 11:44:23 2023, max compression
+gzip compressed data, was "TopasOpt-0.4.4.tar", last modified: Wed Jun 21 05:06:05 2023, max compression
```

## Comparing `TopasOpt-0.4.3.tar` & `TopasOpt-0.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:44:23.182844 TopasOpt-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-06 11:44:23.186843 TopasOpt-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:44:23.182844 TopasOpt-0.4.3/TopasOpt/
--rwxr-xr-x   0 runner    (1001) docker     (123)    52313 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/TopasOpt/Optimisers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/TopasOpt/TopasScriptGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/TopasOpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32339 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/TopasOpt/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:44:23.182844 TopasOpt-0.4.3/TopasOpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 11:44:23.000000 TopasOpt-0.4.3/TopasOpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-06 11:44:23.186843 TopasOpt-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:44:23.182844 TopasOpt-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/tests/test_TopasScriptGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/tests/test_docstring_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/tests/test_optimisers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-06 11:44:14.000000 TopasOpt-0.4.3/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:06:05.971757 TopasOpt-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-21 05:06:05.971757 TopasOpt-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:06:05.971757 TopasOpt-0.4.4/TopasOpt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52313 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/TopasOpt/Optimisers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/TopasOpt/TopasScriptGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/TopasOpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32339 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/TopasOpt/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:06:05.971757 TopasOpt-0.4.4/TopasOpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-21 05:06:05.000000 TopasOpt-0.4.4/TopasOpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 05:06:05.000000 TopasOpt-0.4.4/TopasOpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:06:05.000000 TopasOpt-0.4.4/TopasOpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 05:06:05.000000 TopasOpt-0.4.4/TopasOpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 05:06:05.000000 TopasOpt-0.4.4/TopasOpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-21 05:06:05.971757 TopasOpt-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:06:05.971757 TopasOpt-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/tests/test_TopasScriptGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/tests/test_docstring_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/tests/test_optimisers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 05:05:49.000000 TopasOpt-0.4.4/tests/test_utilities.py
```

### Comparing `TopasOpt-0.4.3/LICENSE.md` & `TopasOpt-0.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.3/PKG-INFO` & `TopasOpt-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopasOpt
-Version: 0.4.3
+Version: 0.4.4
 Summary: optimisation for topas Monte Carlo
 Home-page: https://github.com/ACRF-Image-X-Institute/TopasOpt
 Author: Brendan Whelan
 Author-email: bwheelz360@gmail.com
 Project-URL: Bug Tracker, https://github.com/ACRF-Image-X-Institute/TopasOpt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TopasOpt-0.4.3/README.md` & `TopasOpt-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.3/TopasOpt/Optimisers.py` & `TopasOpt-0.4.4/TopasOpt/Optimisers.py`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.3/TopasOpt/TopasScriptGenerator.py` & `TopasOpt-0.4.4/TopasOpt/TopasScriptGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
             f = open(file)
             TopasScriptGenerator.append('    \n')
             TopasScriptGenerator.append('    ' + ScriptName + ' = []\n')
 
             for line in f:
                 line = line.replace('\n', '')  # remove new line characters
                 CommentLine = False
-                if (not line == '') and line.lstrip()[0] == '#':
+                if (not line.lstrip() == '') and line.lstrip()[0] == '#':
                     CommentLine = True
 
                 if not CommentLine:  # avoid doing anything silly to commented lines
                     line = line.split('#', 1)
                     line = line[0]  # i'm going to remove inline comments, easier and safer.
                     if 'includeFile'.lower() in line.lower():
                         line = self._handle_include_files(file, line)
```

### Comparing `TopasOpt-0.4.3/TopasOpt/utilities.py` & `TopasOpt-0.4.4/TopasOpt/utilities.py`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.3/TopasOpt.egg-info/PKG-INFO` & `TopasOpt-0.4.4/TopasOpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopasOpt
-Version: 0.4.3
+Version: 0.4.4
 Summary: optimisation for topas Monte Carlo
 Home-page: https://github.com/ACRF-Image-X-Institute/TopasOpt
 Author: Brendan Whelan
 Author-email: bwheelz360@gmail.com
 Project-URL: Bug Tracker, https://github.com/ACRF-Image-X-Institute/TopasOpt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TopasOpt-0.4.3/setup.cfg` & `TopasOpt-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.3/tests/test_TopasScriptGenerator.py` & `TopasOpt-0.4.4/tests/test_TopasScriptGenerator.py`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.3/tests/test_docstring_coverage.py` & `TopasOpt-0.4.4/tests/test_docstring_coverage.py`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.3/tests/test_optimisers.py` & `TopasOpt-0.4.4/tests/test_optimisers.py`

 * *Files identical despite different names*

### Comparing `TopasOpt-0.4.3/tests/test_utilities.py` & `TopasOpt-0.4.4/tests/test_utilities.py`

 * *Files identical despite different names*

