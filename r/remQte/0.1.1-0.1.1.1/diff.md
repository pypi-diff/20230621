# Comparing `tmp/remqte-0.1.1.tar.gz` & `tmp/remqte-0.1.1.1.tar.gz`

## Comparing `remqte-0.1.1.tar` & `remqte-0.1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/__init__.py
--rw-r--r--   0        0        0    21863 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/remQte.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/docs/__init__.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/docs/img/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/docs/img/icon.png
--rw-r--r--   0        0        0    19542 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/docs/img/screenshot.png
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/__init__.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/importcsv_s1.ui
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/importcsv_s2.ui
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/importcsv_s3.ui
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/main_scan_choose_nets.ui
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/main_scan_nets.ui
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/main_start.ui
--rw-r--r--   0        0        0    36659 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/remote.ui
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/qtui/img/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/resources/__init__.py
--rw-r--r--   0        0        0    84777 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/resources/images.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 remqte-0.1.1/src/remQte/resources/importzip.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 remqte-0.1.1/LICENSE
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 remqte-0.1.1/README.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 remqte-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 remqte-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/__init__.py
+-rw-r--r--   0        0        0    21863 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/remQte.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/docs/__init__.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/docs/img/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/docs/img/icon.png
+-rw-r--r--   0        0        0    19542 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/docs/img/screenshot.png
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/__init__.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/importcsv_s1.ui
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/importcsv_s2.ui
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/importcsv_s3.ui
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/main_scan_choose_nets.ui
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/main_scan_nets.ui
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/main_start.ui
+-rw-r--r--   0        0        0    36659 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/remote.ui
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/qtui/img/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/resources/__init__.py
+-rw-r--r--   0        0        0    84777 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/resources/images.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 remqte-0.1.1.1/src/remQte/resources/importzip.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 remqte-0.1.1.1/LICENSE
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 remqte-0.1.1.1/README.md
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 remqte-0.1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 remqte-0.1.1.1/PKG-INFO
```

### Comparing `remqte-0.1.1/src/remQte/remQte.py` & `remqte-0.1.1.1/src/remQte/remQte.py`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/docs/img/icon.png` & `remqte-0.1.1.1/src/remQte/docs/img/icon.png`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/docs/img/screenshot.png` & `remqte-0.1.1.1/src/remQte/docs/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/qtui/importcsv_s1.ui` & `remqte-0.1.1.1/src/remQte/qtui/importcsv_s1.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/qtui/importcsv_s2.ui` & `remqte-0.1.1.1/src/remQte/qtui/importcsv_s2.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/qtui/importcsv_s3.ui` & `remqte-0.1.1.1/src/remQte/qtui/importcsv_s3.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/qtui/main_scan_choose_nets.ui` & `remqte-0.1.1.1/src/remQte/qtui/main_scan_choose_nets.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/qtui/main_scan_nets.ui` & `remqte-0.1.1.1/src/remQte/qtui/main_scan_nets.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/qtui/main_start.ui` & `remqte-0.1.1.1/src/remQte/qtui/main_start.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/qtui/remote.ui` & `remqte-0.1.1.1/src/remQte/qtui/remote.ui`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/resources/images.py` & `remqte-0.1.1.1/src/remQte/resources/images.py`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/src/remQte/resources/importzip.py` & `remqte-0.1.1.1/src/remQte/resources/importzip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import zipfile, io, os
 import sqlite3, codecs
 import tempfile
-tmpdir = tempfile.gettempdir()+'\\remQte\\'
+tmpdir = tempfile.gettempdir()+'/remQte'
 if not os.path.exists(tmpdir):
     os.makedirs(tmpdir)
 #print(tmpdir)
 class channels:
     chnnls = []
     def add(self,row):
         itm = {'channel':row[0],'name':row[1],'type':'tv'}
```

### Comparing `remqte-0.1.1/LICENSE` & `remqte-0.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/README.md` & `remqte-0.1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `remqte-0.1.1/pyproject.toml` & `remqte-0.1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "remQte"
-version = "0.1.1"
+version = "0.1.1.1"
 authors = [{ name="Philipp M. Nöhren", email="remQte@proton.me" }]
 description = "Remote-control GUI for Samsung Smart TVs, newer than 2016."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: End Users/Desktop",
```

### Comparing `remqte-0.1.1/PKG-INFO` & `remqte-0.1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remQte
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: Remote-control GUI for Samsung Smart TVs, newer than 2016.
 Project-URL: Homepage, https://github.com/barfnordsen/remQte
 Project-URL: Bug Tracker, https://github.com/barfnordsen/remQte/issues
 Author-email: "Philipp M. Nöhren" <remQte@proton.me>
 License-File: LICENSE
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

