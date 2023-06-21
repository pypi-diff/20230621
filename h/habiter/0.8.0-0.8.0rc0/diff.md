# Comparing `tmp/habiter-0.8.0.tar.gz` & `tmp/habiter-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habiter-0.8.0.tar", last modified: Wed Jun 21 21:12:24 2023, max compression
+gzip compressed data, was "habiter-0.8.0rc0.tar", last modified: Wed Jun 21 21:09:22 2023, max compression
```

## Comparing `habiter-0.8.0.tar` & `habiter-0.8.0rc0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.228838 habiter-0.8.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-06-21 19:28:09.000000 habiter-0.8.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6706 2023-06-21 21:12:24.228838 habiter-0.8.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6258 2023-06-21 19:28:09.000000 habiter-0.8.0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.218838 habiter-0.8.0/habiter/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       22 2023-06-21 21:12:17.000000 habiter-0.8.0/habiter/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.228838 habiter-0.8.0/habiter/api/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1471 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/api/export.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.228838 habiter-0.8.0/habiter/internal/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      557 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/cli.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.228838 habiter-0.8.0/habiter/internal/commands/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/commands/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       77 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/commands/_utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1528 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/commands/add.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2844 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/commands/list.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1248 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/commands/remove.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1649 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/commands/reset.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2737 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/commands/tally.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.228838 habiter-0.8.0/habiter/internal/file/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/file/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2583 2023-06-21 20:39:09.000000 habiter-0.8.0/habiter/internal/file/creator.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1417 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/file/operations.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2764 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/file/updater.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1926 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/math.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      877 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/run.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.228838 habiter-0.8.0/habiter/internal/utils/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/utils/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      109 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/utils/consts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2023-06-21 19:28:09.000000 habiter-0.8.0/habiter/internal/utils/messenger.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.228838 habiter-0.8.0/habiter.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6706 2023-06-21 21:12:24.000000 habiter-0.8.0/habiter.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-06-21 21:12:24.000000 habiter-0.8.0/habiter.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-21 21:12:24.000000 habiter-0.8.0/habiter.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-06-21 21:12:24.000000 habiter-0.8.0/habiter.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      133 2023-06-21 21:12:24.000000 habiter-0.8.0/habiter.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-06-21 21:12:24.000000 habiter-0.8.0/habiter.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      899 2023-06-21 21:12:24.228838 habiter-0.8.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-21 19:28:09.000000 habiter-0.8.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:12:24.228838 habiter-0.8.0/test/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      902 2023-06-21 19:28:09.000000 habiter-0.8.0/test/test_add.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1311 2023-06-21 19:28:09.000000 habiter-0.8.0/test/test_list.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      695 2023-06-21 19:28:09.000000 habiter-0.8.0/test/test_remove.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1229 2023-06-21 19:28:09.000000 habiter-0.8.0/test/test_reset.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2149 2023-06-21 19:28:09.000000 habiter-0.8.0/test/test_tally.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.331341 habiter-0.8.0rc0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6709 2023-06-21 21:09:22.331341 habiter-0.8.0rc0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6258 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.321341 habiter-0.8.0rc0/habiter/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-21 21:09:17.000000 habiter-0.8.0rc0/habiter/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.321341 habiter-0.8.0rc0/habiter/api/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/api/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1471 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/api/export.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.321341 habiter-0.8.0rc0/habiter/internal/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      557 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/cli.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.331341 habiter-0.8.0rc0/habiter/internal/commands/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/commands/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       77 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/commands/_utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1528 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/commands/add.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2844 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/commands/list.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1248 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/commands/remove.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1649 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/commands/reset.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2737 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/commands/tally.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.331341 habiter-0.8.0rc0/habiter/internal/file/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/file/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2583 2023-06-21 20:39:09.000000 habiter-0.8.0rc0/habiter/internal/file/creator.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1417 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/file/operations.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2764 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/file/updater.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1926 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/math.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      877 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/run.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.331341 habiter-0.8.0rc0/habiter/internal/utils/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/utils/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      109 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/utils/consts.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/habiter/internal/utils/messenger.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.321341 habiter-0.8.0rc0/habiter.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6709 2023-06-21 21:09:22.000000 habiter-0.8.0rc0/habiter.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-06-21 21:09:22.000000 habiter-0.8.0rc0/habiter.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-21 21:09:22.000000 habiter-0.8.0rc0/habiter.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-06-21 21:09:22.000000 habiter-0.8.0rc0/habiter.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      133 2023-06-21 21:09:22.000000 habiter-0.8.0rc0/habiter.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-06-21 21:09:22.000000 habiter-0.8.0rc0/habiter.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      899 2023-06-21 21:09:22.331341 habiter-0.8.0rc0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 21:09:22.331341 habiter-0.8.0rc0/test/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      902 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/test/test_add.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1311 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/test/test_list.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      695 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/test/test_remove.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1229 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/test/test_reset.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2149 2023-06-21 19:28:09.000000 habiter-0.8.0rc0/test/test_tally.py
```

### Comparing `habiter-0.8.0/LICENSE` & `habiter-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/PKG-INFO` & `habiter-0.8.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habiter
-Version: 0.8.0
+Version: 0.8.0rc0
 Summary: Quantifiy and keep tabs on habits.
 Home-page: https://github.com/kemzeb/habiter
 Author: Kemal Zebari
 License: MIT
 Keywords: productivity,cli
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `habiter-0.8.0/README.md` & `habiter-0.8.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/api/export.py` & `habiter-0.8.0rc0/habiter/api/export.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/cli.py` & `habiter-0.8.0rc0/habiter/internal/cli.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/commands/add.py` & `habiter-0.8.0rc0/habiter/internal/commands/add.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/commands/list.py` & `habiter-0.8.0rc0/habiter/internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/commands/remove.py` & `habiter-0.8.0rc0/habiter/internal/commands/remove.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/commands/reset.py` & `habiter-0.8.0rc0/habiter/internal/commands/reset.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/commands/tally.py` & `habiter-0.8.0rc0/habiter/internal/commands/tally.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/file/creator.py` & `habiter-0.8.0rc0/habiter/internal/file/creator.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/file/operations.py` & `habiter-0.8.0rc0/habiter/internal/file/operations.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/file/updater.py` & `habiter-0.8.0rc0/habiter/internal/file/updater.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/math.py` & `habiter-0.8.0rc0/habiter/internal/math.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/run.py` & `habiter-0.8.0rc0/habiter/internal/run.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter/internal/utils/messenger.py` & `habiter-0.8.0rc0/habiter/internal/utils/messenger.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/habiter.egg-info/PKG-INFO` & `habiter-0.8.0rc0/habiter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habiter
-Version: 0.8.0
+Version: 0.8.0rc0
 Summary: Quantifiy and keep tabs on habits.
 Home-page: https://github.com/kemzeb/habiter
 Author: Kemal Zebari
 License: MIT
 Keywords: productivity,cli
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `habiter-0.8.0/habiter.egg-info/SOURCES.txt` & `habiter-0.8.0rc0/habiter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/setup.cfg` & `habiter-0.8.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/test/test_add.py` & `habiter-0.8.0rc0/test/test_add.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/test/test_list.py` & `habiter-0.8.0rc0/test/test_list.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/test/test_remove.py` & `habiter-0.8.0rc0/test/test_remove.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/test/test_reset.py` & `habiter-0.8.0rc0/test/test_reset.py`

 * *Files identical despite different names*

### Comparing `habiter-0.8.0/test/test_tally.py` & `habiter-0.8.0rc0/test/test_tally.py`

 * *Files identical despite different names*

