# Comparing `tmp/bitmap2-0.2.2.tar.gz` & `tmp/bitmap2-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmap2-0.2.2.tar", last modified: Tue Apr 18 16:43:18 2023, max compression
+gzip compressed data, was "bitmap2-0.2.3.tar", last modified: Wed Jun 21 17:33:37 2023, max compression
```

## Comparing `bitmap2-0.2.2.tar` & `bitmap2-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-18 16:43:12.000000 bitmap2-0.2.2/.github/workflows/pypi-upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-18 16:43:12.000000 bitmap2-0.2.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-18 16:43:12.000000 bitmap2-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 16:43:12.000000 bitmap2-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 16:43:12.000000 bitmap2-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 16:43:18.679307 bitmap2-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-18 16:43:12.000000 bitmap2-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/bitmap2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 16:43:18.000000 bitmap2-0.2.2/bitmap2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 16:43:18.000000 bitmap2-0.2.2/bitmap2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:43:18.000000 bitmap2-0.2.2/bitmap2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:43:18.000000 bitmap2-0.2.2/bitmap2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:43:18.679307 bitmap2-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-04-18 16:43:12.000000 bitmap2-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 16:43:12.000000 bitmap2-0.2.2/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6595 2023-04-18 16:43:12.000000 bitmap2-0.2.2/src/bitmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-04-18 16:43:12.000000 bitmap2-0.2.2/test/test_bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.443524 bitmap2-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 17:33:32.000000 bitmap2-0.2.3/.github/workflows/pypi-upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-21 17:33:32.000000 bitmap2-0.2.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-21 17:33:32.000000 bitmap2-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 17:33:32.000000 bitmap2-0.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 17:33:32.000000 bitmap2-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-21 17:33:37.443524 bitmap2-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-21 17:33:32.000000 bitmap2-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/bitmap2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-21 17:33:37.000000 bitmap2-0.2.3/bitmap2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 17:33:37.000000 bitmap2-0.2.3/bitmap2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:33:37.000000 bitmap2-0.2.3/bitmap2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 17:33:37.000000 bitmap2-0.2.3/bitmap2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:33:37.443524 bitmap2-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-06-21 17:33:32.000000 bitmap2-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 17:33:32.000000 bitmap2-0.2.3/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6595 2023-06-21 17:33:32.000000 bitmap2-0.2.3/src/bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:33:37.439523 bitmap2-0.2.3/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-06-21 17:33:32.000000 bitmap2-0.2.3/test/test_bitmap.py
```

### Comparing `bitmap2-0.2.2/.github/workflows/pypi-upload.yml` & `bitmap2-0.2.3/.github/workflows/pypi-upload.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.2/.github/workflows/test.yml` & `bitmap2-0.2.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.2/.gitignore` & `bitmap2-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.2/LICENSE.md` & `bitmap2-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.2/PKG-INFO` & `bitmap2-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.2
+Version: 0.2.3
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.2/README.md` & `bitmap2-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.2/bitmap2.egg-info/PKG-INFO` & `bitmap2-0.2.3/bitmap2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.2
+Version: 0.2.3
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.2/setup.py` & `bitmap2-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.2/src/bitmap.py` & `bitmap2-0.2.3/src/bitmap.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -248,13 +248,13 @@
     def fromfile(cls, path, maxnum=None):
         if maxnum is None:
             with open(path, 'rb') as file:
                 bitmap = file.read()
             return cls(bitmap=bitmap)
         else:
             bm = cls(maxnum)
-            bm.bitmap = array.array('B')
             file = open(path, 'rb')
+            bm.bitmap = array.array('B')
             bm.bitmap.fromfile(file, (maxnum + 7) // 8)
             file.close()
             return bm
```

### Comparing `bitmap2-0.2.2/test/test_bitmap.py` & `bitmap2-0.2.3/test/test_bitmap.py`

 * *Files identical despite different names*

