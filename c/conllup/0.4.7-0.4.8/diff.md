# Comparing `tmp/conllup-0.4.7.tar.gz` & `tmp/conllup-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conllup-0.4.7.tar", last modified: Fri Jun 16 09:08:55 2023, max compression
+gzip compressed data, was "conllup-0.4.8.tar", last modified: Wed Jun 21 07:15:33 2023, max compression
```

## Comparing `conllup-0.4.7.tar` & `conllup-0.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-16 09:08:55.405999 conllup-0.4.7/
--rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-06-16 09:08:55.405999 conllup-0.4.7/PKG-INFO
--rw-rw-r--   0 wran      (1000) wran      (1000)     3499 2023-04-18 13:19:26.000000 conllup-0.4.7/README.md
--rw-rw-r--   0 wran      (1000) wran      (1000)       24 2023-02-01 16:20:21.000000 conllup-0.4.7/long_description.rst
--rw-rw-r--   0 wran      (1000) wran      (1000)      246 2023-06-16 09:08:21.000000 conllup-0.4.7/pyproject.toml
--rw-rw-r--   0 wran      (1000) wran      (1000)      482 2023-06-16 09:08:55.405999 conllup-0.4.7/setup.cfg
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-16 09:08:55.401999 conllup-0.4.7/src/
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-16 09:08:55.405999 conllup-0.4.7/src/conllup/
--rw-rw-r--   0 wran      (1000) wran      (1000)        0 2023-01-30 16:14:25.000000 conllup-0.4.7/src/conllup/__init__.py
--rw-rw-r--   0 wran      (1000) wran      (1000)    11986 2023-06-16 09:06:17.000000 conllup-0.4.7/src/conllup/conllup.py
--rw-rw-r--   0 wran      (1000) wran      (1000)     6856 2023-04-18 13:11:48.000000 conllup-0.4.7/src/conllup/processing.py
--rw-rw-r--   0 wran      (1000) wran      (1000)      570 2023-04-18 13:10:04.000000 conllup-0.4.7/src/conllup/types.py
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-16 09:08:55.405999 conllup-0.4.7/src/conllup.egg-info/
--rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-06-16 09:08:55.000000 conllup-0.4.7/src/conllup.egg-info/PKG-INFO
--rw-rw-r--   0 wran      (1000) wran      (1000)      289 2023-06-16 09:08:55.000000 conllup-0.4.7/src/conllup.egg-info/SOURCES.txt
--rw-rw-r--   0 wran      (1000) wran      (1000)        1 2023-06-16 09:08:55.000000 conllup-0.4.7/src/conllup.egg-info/dependency_links.txt
--rw-rw-r--   0 wran      (1000) wran      (1000)        8 2023-06-16 09:08:55.000000 conllup-0.4.7/src/conllup.egg-info/top_level.txt
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-21 07:15:33.636364 conllup-0.4.8/
+-rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-06-21 07:15:33.636364 conllup-0.4.8/PKG-INFO
+-rw-rw-r--   0 wran      (1000) wran      (1000)     3793 2023-06-21 07:03:45.000000 conllup-0.4.8/README.md
+-rw-rw-r--   0 wran      (1000) wran      (1000)       24 2023-02-01 16:20:21.000000 conllup-0.4.8/long_description.rst
+-rw-rw-r--   0 wran      (1000) wran      (1000)      246 2023-06-21 07:15:13.000000 conllup-0.4.8/pyproject.toml
+-rw-rw-r--   0 wran      (1000) wran      (1000)      482 2023-06-21 07:15:33.640364 conllup-0.4.8/setup.cfg
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-21 07:15:33.636364 conllup-0.4.8/src/
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-21 07:15:33.636364 conllup-0.4.8/src/conllup/
+-rw-rw-r--   0 wran      (1000) wran      (1000)        0 2023-01-30 16:14:25.000000 conllup-0.4.8/src/conllup/__init__.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)    12236 2023-06-21 07:09:25.000000 conllup-0.4.8/src/conllup/conllup.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)     6856 2023-04-18 13:11:48.000000 conllup-0.4.8/src/conllup/processing.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)      570 2023-04-18 13:10:04.000000 conllup-0.4.8/src/conllup/types.py
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-21 07:15:33.636364 conllup-0.4.8/src/conllup.egg-info/
+-rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-06-21 07:15:33.000000 conllup-0.4.8/src/conllup.egg-info/PKG-INFO
+-rw-rw-r--   0 wran      (1000) wran      (1000)      289 2023-06-21 07:15:33.000000 conllup-0.4.8/src/conllup.egg-info/SOURCES.txt
+-rw-rw-r--   0 wran      (1000) wran      (1000)        1 2023-06-21 07:15:33.000000 conllup-0.4.8/src/conllup.egg-info/dependency_links.txt
+-rw-rw-r--   0 wran      (1000) wran      (1000)        8 2023-06-21 07:15:33.000000 conllup-0.4.8/src/conllup.egg-info/top_level.txt
```

### Comparing `conllup-0.4.7/README.md` & `conllup-0.4.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,19 @@
 
 1. change versions in pyproject.toml
 2. build new package `python3 -m build`
 3. upload to pypi `python3 -m twine upload --repository pypi dist/*`
 4. Optional : if you want to try the testpypi version of the package `pip install --index-url https://test.pypi.org/simple/ --no-deps conllup`
 
 ## Changelog
+### 0.4.8
+- raise errors for empty tokens
+### 0.4.7
+- modify _featuresConllToJson() so it order features in the order [specified by UD](https://universaldependencies.org/format.html) (thank you @bguil): 
+> In sorting, uppercase letters are considered identical to their lowercase counterparts.
 ### 0.4.6
 - add order in place in replaceArrayOfTokens() outputted treeJson (thanks to the new _sortTokensJson())
 ### 0.4.4:
 - minor fix
 ### 0.4.3:
 - optimized for speed (reduced by half the time of loading and serializing conllus)
 ### 0.4.2:
```

### Comparing `conllup-0.4.7/src/conllup/conllup.py` & `conllup-0.4.8/src/conllup/conllup.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,21 @@
     trimmedNodeConll = nodeConll.rstrip().strip()
     splittedNodeConll = trimmedNodeConll.split("\t")
     if len(splittedNodeConll) != 10:
         raise Exception(
             f'COLUMNS NUMBER ERROR : {len(splittedNodeConll)} columns found instead of 10  --- line content = "{nodeConll}"'
         )
 
+    empty_columns = [i+1 for i, x in enumerate(splittedNodeConll) if x == ""]
+
+    if len(empty_columns) > 0:
+        raise Exception(
+            f'EMPTY COLUMN ERROR : columns {empty_columns} are empty  --- line content = "{nodeConll}"'
+        )
+
     tokenJson = {
         "ID": splittedNodeConll[0],
         "FORM": splittedNodeConll[1],
         "LEMMA": splittedNodeConll[2],
         "UPOS": splittedNodeConll[3],
         "XPOS": splittedNodeConll[4],
         "FEATS": _featuresConllToJson(splittedNodeConll[5]),
```

### Comparing `conllup-0.4.7/src/conllup/processing.py` & `conllup-0.4.8/src/conllup/processing.py`

 * *Files identical despite different names*

### Comparing `conllup-0.4.7/src/conllup/types.py` & `conllup-0.4.8/src/conllup/types.py`

 * *Files identical despite different names*

