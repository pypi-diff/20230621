# Comparing `tmp/SummarizedExperiment-0.2.4.tar.gz` & `tmp/SummarizedExperiment-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SummarizedExperiment-0.2.4.tar", last modified: Thu Mar 23 07:40:08 2023, max compression
+gzip compressed data, was "SummarizedExperiment-0.2.5.tar", last modified: Wed Jun 21 17:31:12 2023, max compression
```

## Comparing `SummarizedExperiment-0.2.4.tar` & `SummarizedExperiment-0.2.5.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.167080 SummarizedExperiment-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.159080 SummarizedExperiment-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.163081 SummarizedExperiment-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-23 07:40:08.167080 SummarizedExperiment-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.163081 SummarizedExperiment-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.163081 SummarizedExperiment-0.2.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-23 07:40:08.167080 SummarizedExperiment-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.159080 SummarizedExperiment-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.167080 SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-23 07:40:08.000000 SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-23 07:40:08.000000 SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 07:40:08.000000 SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 07:39:06.000000 SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-23 07:40:08.000000 SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 07:40:08.000000 SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.167080 SummarizedExperiment-0.2.4/src/summarizedexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/src/summarizedexperiment/BaseSE.py
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/src/summarizedexperiment/RangeSummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/src/summarizedexperiment/SummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/src/summarizedexperiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:40:08.167080 SummarizedExperiment-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/tests/test_RSE.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/tests/test_RSE_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/tests/test_SE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/tests/test_SE_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-23 07:38:58.000000 SummarizedExperiment-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.390227 SummarizedExperiment-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.398227 SummarizedExperiment-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.402227 SummarizedExperiment-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.402227 SummarizedExperiment-0.2.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 17:31:12.410227 SummarizedExperiment-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.394227 SummarizedExperiment-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.402227 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:29:45.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/src/summarizedexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15507 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/BaseSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23312 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/RangeSummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/RangedSummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/SummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/data/tenx.sub.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_RSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_RSE_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_SE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_SE_backed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_SE_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tox.ini
```

### Comparing `SummarizedExperiment-0.2.4/.coveragerc` & `SummarizedExperiment-0.2.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/.github/workflows/pypi-publish.yml` & `SummarizedExperiment-0.2.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/.github/workflows/pypi-test.yml` & `SummarizedExperiment-0.2.5/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/.gitignore` & `SummarizedExperiment-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/CHANGELOG.md` & `SummarizedExperiment-0.2.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/CONTRIBUTING.rst` & `SummarizedExperiment-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/LICENSE.txt` & `SummarizedExperiment-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/PKG-INFO` & `SummarizedExperiment-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SummarizedExperiment
-Version: 0.2.4
+Version: 0.2.5
 Summary: Container to represent data from genomic experiments
 Home-page: https://github.com/BiocPy/summarizedexperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/summarizedexperiment
 Platform: any
```

### Comparing `SummarizedExperiment-0.2.4/README.md` & `SummarizedExperiment-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/docs/Makefile` & `SummarizedExperiment-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/docs/changelog.md` & `SummarizedExperiment-0.2.5/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/docs/conf.py` & `SummarizedExperiment-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/docs/index.md` & `SummarizedExperiment-0.2.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/docs/readme.md` & `SummarizedExperiment-0.2.5/docs/readme.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/docs/tutorial.md` & `SummarizedExperiment-0.2.5/docs/tutorial.md`

 * *Files 21% similar despite different names*

```diff
@@ -57,14 +57,53 @@
 
 ```python
 tse = SummarizedExperiment(
     assays={"counts": counts}, rowData=df_gr, colData=colData
 )
 ```
 
+### File backed mode for large datasets
+
+In addition to fully realized matrices in memory, SE/RSE also support file backed arrays and matrices. [FileBackedArray](https://github.com/BiocPy/FileBackedArray) package provides a file backed class for H5 backed matrices.
+
+```python
+df_gr = pd.DataFrame(
+    {
+        "seqnames": [
+            "chr1",
+            "chr2",
+            "chr2",
+            "chr2",
+            "chr1",
+            "chr1",
+            "chr3",
+            "chr3",
+            "chr3",
+            "chr3",
+        ]
+        * 100,
+        "starts": range(0, 1000),
+        "ends": range(0, 1000),
+        "strand": ["-", "+", "+", "*", "*", "+", "+", "+", "-", "-"] * 100,
+        "score": range(0, 1000),
+        "GC": [random() for _ in range(10)] * 100,
+    }
+)
+
+colData = pd.DataFrame({"treatment": ["ChIP"] * 3005,})
+
+assay = H5BackedData("tests/data/tenx.sub.h5", "matrix")
+
+tse = SummarizedExperiment(
+    assays={"counts_backed": assay},
+    rowData=df_gr,
+    colData=colData,
+)
+```
+
 ##  `RangeSummarizedExperiment`
 
 `RangeSummarizedExperiment` represents features as [`GenomicRanges`](https://github.com/BiocPy/GenomicRanges).
 
 ```python
 gr = GenomicRanges.fromPandas(df_gr)
 
@@ -102,8 +141,9 @@
 query = {"seqnames": ["chr2",], "starts": [4], "ends": [6], "strand": ["+"]}
 
 query = GenomicRanges(query)
 
 tse.subsetOverlaps(query)
 ```
 
-Checkout the API docs or GenomicRanges for list of interval based operations.
+Checkout the API docs or GenomicRanges for list of interval based operations.
+
```

### Comparing `SummarizedExperiment-0.2.4/setup.cfg` & `SummarizedExperiment-0.2.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
+	biocframe>=0.2.13
 	genomicranges>=0.2.9
+	filebackedarray>=0.0.2
 	scipy
 	anndata
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `SummarizedExperiment-0.2.4/setup.py` & `SummarizedExperiment-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/PKG-INFO` & `SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SummarizedExperiment
-Version: 0.2.4
+Version: 0.2.5
 Summary: Container to represent data from genomic experiments
 Home-page: https://github.com/BiocPy/summarizedexperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/summarizedexperiment
 Platform: any
```

### Comparing `SummarizedExperiment-0.2.4/src/SummarizedExperiment.egg-info/SOURCES.txt` & `SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 src/SummarizedExperiment.egg-info/SOURCES.txt
 src/SummarizedExperiment.egg-info/dependency_links.txt
 src/SummarizedExperiment.egg-info/not-zip-safe
 src/SummarizedExperiment.egg-info/requires.txt
 src/SummarizedExperiment.egg-info/top_level.txt
 src/summarizedexperiment/BaseSE.py
 src/summarizedexperiment/RangeSummarizedExperiment.py
+src/summarizedexperiment/RangedSummarizedExperiment.py
 src/summarizedexperiment/SummarizedExperiment.py
 src/summarizedexperiment/__init__.py
 tests/conftest.py
 tests/test_RSE.py
 tests/test_RSE_methods.py
 tests/test_SE.py
-tests/test_SE_methods.py
+tests/test_SE_backed.py
+tests/test_SE_methods.py
+tests/data/tenx.sub.h5
```

### Comparing `SummarizedExperiment-0.2.4/src/summarizedexperiment/BaseSE.py` & `SummarizedExperiment-0.2.5/src/summarizedexperiment/BaseSE.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,76 +1,83 @@
-from typing import Union, MutableMapping, Sequence, Tuple, Optional
+from collections import OrderedDict
+from typing import MutableMapping, Optional, Sequence, Tuple, Union
+
+import anndata
+import numpy as np
+import pandas as pd
 from biocframe import BiocFrame
 from genomicranges import GenomicRanges
 from scipy import sparse as sp
-import numpy as np
-import pandas as pd
-from collections import OrderedDict
-import anndata
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 class BaseSE:
     """Base class for Summarized Experiment.
-    
-    Represents genomic experiment data (`assays`), features (`rowdata`), 
+
+    Represents genomic experiment data (`assays`), features (`rowdata`),
     sample data (`coldata`) and any other metadata.
+
+    Args:
+        assays (MutableMapping[str, Union[np.ndarray, sp.spmatrix]]): dictionary
+            of matrices, with assay names as keys and matrices represented as dense
+            (numpy) or sparse (scipy) matrices. All matrices across assays must
+            have the same dimensions (number of rows, number of columns).
+        rowData (GenomicRanges, optional): features, must be the same length as
+            rows of the matrices in assays. Defaults to None.
+        colData (Union[pd.DataFrame, BiocFrame], optional): sample data, must be
+            the same length as rows of the matrices in assays. Defaults to None.
+        metadata (MutableMapping, optional): experiment metadata describing the
+            methods. Defaults to None.
     """
 
+    # TODO: should be an instance attribute 
     _shape = None
 
     def __init__(
         self,
         assays: MutableMapping[str, Union[np.ndarray, sp.spmatrix]],
         rows: Optional[Union[pd.DataFrame, BiocFrame]] = None,
         cols: Optional[Union[pd.DataFrame, BiocFrame]] = None,
         metadata: Optional[MutableMapping] = None,
     ) -> None:
-        """Initialize an instance of `BaseSE`.
-
-        Args:
-            assays (MutableMapping[str, Union[np.ndarray, sp.spmatrix]]): dictionary 
-                of matrices, with assay names as keys and matrices represented as dense 
-                (numpy) or sparse (scipy) matrices. All matrices across assays must 
-                have the same dimensions (number of rows, number of columns).
-            rowData (GenomicRanges, optional): features, must be the same length as 
-                rows of the matrices in assays. Defaults to None.
-            colData (Union[pd.DataFrame, BiocFrame], optional): sample data, must be 
-                the same length as rows of the matrices in assays. Defaults to None.
-            metadata (MutableMapping, optional): experiment metadata describing the 
-                methods. Defaults to None.
-        """
+        """Initialize an instance of `BaseSE`."""
 
         if assays is None or not isinstance(assays, dict) or len(assays.keys()) == 0:
             raise Exception(
                 f"{assays} must be a dictionary and contain "
                 "atleast one matrix (either sparse or dense)"
             )
 
         self._validate_assays(assays)
         self._assays = assays
 
+        # should have _shape by now
+        if self._shape is None:
+            raise TypeError(
+                "This should not happen; ssays is not consistent. "
+                "Report this issue with a reproducible example!"
+            )
+
         rows = rows if rows is not None else BiocFrame({}, numberOfRows=self._shape[0])
         self._validate_rows(rows)
         self._rows = rows
 
         cols = cols if cols is not None else BiocFrame({}, numberOfRows=self._shape[1])
         self._validate_cols(cols)
         self._cols = (
             cols if cols is not None else BiocFrame({}, numberOfRows=self._shape[1])
         )
 
         self._metadata = metadata
 
     def _validate(self):
-        """Internal wrapper method to validate the object.
-        """
+        """Internal wrapper method to validate the object."""
         # validate assays to make sure they are have same dimensions
         self._validate_assays(self._assays)
         self._validate_rows(self._rows)
         self._validate_cols(self._cols)
 
     def _validate_assays(
         self, assays: MutableMapping[str, Union[np.ndarray, sp.spmatrix]]
@@ -82,14 +89,19 @@
                 data.
 
         Raises:
             ValueError: when assays contain more than 2 dimensions.
             ValueError: if all assays do not have the same dimensions.
         """
         for asy, mat in assays.items():
+            print("asy_name", asy)
+            print(mat)
+            print(mat.shape)
+            print(self._shape)
+
             if len(mat.shape) > 2:
                 raise ValueError(
                     "only 2-dimensional matrices are accepted, "
                     f"provided {len(mat.shape)} dimensions for assay {asy}"
                 )
 
             if self._shape is None:
@@ -102,15 +114,15 @@
                     f" but provided {mat.shape}"
                 )
 
     def _validate_rows(self, rows: Optional[Union[pd.DataFrame, BiocFrame]]):
         """Internal method to validate feature information (rowdata).
 
         Args:
-            rows (Optional[Union[pd.DataFrame, BiocFrame]]): feature information 
+            rows (Optional[Union[pd.DataFrame, BiocFrame]]): feature information
                 (rowdata).
 
         Raises:
             ValueError: when number of rows does not match between rows & assays.
             TypeError: when rows is neither a pandas dataframe not Biocframe object.
         """
         if not (isinstance(rows, pd.DataFrame) or isinstance(rows, BiocFrame)):
@@ -125,15 +137,15 @@
                 f" but provided {rows.shape[0]}"
             )
 
     def _validate_cols(self, cols: Optional[Union[pd.DataFrame, BiocFrame]]):
         """Internal method to validate sample information (coldata).
 
         Args:
-            cols (Optional[Union[pd.DataFrame, BiocFrame]]): sample information 
+            cols (Optional[Union[pd.DataFrame, BiocFrame]]): sample information
                 (coldata).
 
         Raises:
             ValueError: when number of samples do not match between cols & assays.
             TypeError: when cols is neither a pandas dataframe not Biocframe object.
         """
         if not (isinstance(cols, pd.DataFrame) or isinstance(cols, BiocFrame)):
@@ -149,15 +161,15 @@
             )
 
     @property
     def assays(self) -> MutableMapping[str, Union[np.ndarray, sp.spmatrix]]:
         """Get assays.
 
         Returns:
-            MutableMapping[str, Union[np.ndarray, sp.spmatrix]]: a dictionary with  
+            MutableMapping[str, Union[np.ndarray, sp.spmatrix]]: a dictionary with
             experiments names as keys and matrix data as values.
         """
         return self._assays
 
     @assays.setter
     def assays(
         self, assays: MutableMapping[str, Union[np.ndarray, sp.spmatrix]]
@@ -290,17 +302,17 @@
         self,
         rowIndices: Optional[Union[Sequence[int], slice]] = None,
         colIndices: Optional[Union[Sequence[int], slice]] = None,
     ) -> MutableMapping[str, Union[np.ndarray, sp.spmatrix]]:
         """Subset all assays to a specified set of {rows, cols or both} slices.
 
         Args:
-            rowIndices (Union[Sequence[int], slice], optional): row indices to subset. 
+            rowIndices (Union[Sequence[int], slice], optional): row indices to subset.
                 Defaults to None.
-            colIndices (Union[Sequence[int], slice], optional): col indices to subset. 
+            colIndices (Union[Sequence[int], slice], optional): col indices to subset.
                 Defaults to None.
 
         Raises:
             ValueError: if `rowIndices` and `colIndices` are both None.
 
         Returns:
             MutableMapping[str, Union[np.ndarray, sp.spmatrix]]: experiment data
@@ -329,22 +341,22 @@
         Union[pd.DataFrame, BiocFrame],
         Union[pd.DataFrame, BiocFrame],
         MutableMapping[str, Union[np.ndarray, sp.spmatrix]],
     ]:
         """Internal method to slice `SE` by index.
 
         Args:
-            args (Tuple[Union[Sequence[int], slice], Optional[Union[Sequence[int], slice]]]): 
+            args (Tuple[Union[Sequence[int], slice], Optional[Union[Sequence[int], slice]]]):
                 indices to slice. tuple contains slices along dimensions (rows, cols).
 
         Raises:
             ValueError: Too many or too few slices provided.
 
         Returns:
-            Tuple[Union[pd.DataFrame, BiocFrame], Union[pd.DataFrame, BiocFrame], MutableMapping[str, Union[np.ndarray, sp.spmatrix]]]: 
+            Tuple[Union[pd.DataFrame, BiocFrame], Union[pd.DataFrame, BiocFrame], MutableMapping[str, Union[np.ndarray, sp.spmatrix]]]:
             sliced row, cols and assays.
         """
 
         if len(args) == 0:
             raise ValueError("Arguments must contain one slice")
 
         rowIndices = args[0]
@@ -432,27 +444,32 @@
             )
 
         if isinstance(self._cols, pd.DataFrame):
             self._cols.index = names
         else:
             self._cols.rowNames = names
 
-    def toAnnData(self,) -> anndata.AnnData:
-        """Transform `SummarizedExperiment` to `AnnData` representation. 
+    def toAnnData(
+        self,
+    ) -> anndata.AnnData:
+        """Transform `SummarizedExperiment` to `AnnData` representation.
 
         Returns:
             anndata.AnnData: returns an `AnnData` representation of SE.
         """
 
         layers = OrderedDict()
         for asy, mat in self.assays.items():
             layers[asy] = mat.transpose()
 
         trows = self._rows
         if isinstance(self._rows, GenomicRanges):
             trows = self._rows.toPandas()
 
         obj = anndata.AnnData(
-            obs=self._cols, var=trows, uns=self.metadata, layers=layers,
+            obs=self._cols,
+            var=trows,
+            uns=self.metadata,
+            layers=layers,
         )
 
         return obj
```

### Comparing `SummarizedExperiment-0.2.4/src/summarizedexperiment/RangeSummarizedExperiment.py` & `SummarizedExperiment-0.2.5/src/summarizedexperiment/RangeSummarizedExperiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Union, Tuple, Sequence, Optional, MutableMapping
-import pandas as pd
-import numpy as np
-from scipy import sparse as sp
+from typing import MutableMapping, Optional, Sequence, Tuple, Union
 
+import numpy as np
+import pandas as pd
 from biocframe import BiocFrame
 from genomicranges import GenomicRanges, SeqInfo
+from scipy import sparse as sp
 
 from .BaseSE import BaseSE
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
@@ -24,31 +24,31 @@
         rowRanges: Optional[GenomicRanges],
         colData: Optional[Union[pd.DataFrame, BiocFrame]] = None,
         metadata: Optional[MutableMapping] = None,
     ) -> None:
         """Initialize a Range Summarized Experiment (RSE) object.
 
         The key difference between this and `SummarizedExperiment` is enforcing
-        type for feature information (`rowRanges`), must be a `GenomicRanges` object. 
+        type for feature information (`rowRanges`), must be a `GenomicRanges` object.
         This allows us to provides new methods, to perform genomic range based
         operations over experimental data.
 
-        Note: If `rowRanges` is empty, None or not a genomic ranges object, 
+        Note: If `rowRanges` is empty, None or not a genomic ranges object,
         use a `SummarizedExperiment` instead!
 
         Args:
-            assays (MutableMapping[str, Union[np.ndarray, sp.spmatrix]]): dictionary 
-                of matrices, with assay names as keys and matrices represented as dense 
-                (numpy) or sparse (scipy) matrices. All matrices across assays must 
+            assays (MutableMapping[str, Union[np.ndarray, sp.spmatrix]]): dictionary
+                of matrices, with assay names as keys and matrices represented as dense
+                (numpy) or sparse (scipy) matrices. All matrices across assays must
                 have the same dimensions (number of rows, number of columns).
-            rowRanges (GenomicRanges): features, must be the same length as 
+            rowRanges (GenomicRanges): features, must be the same length as
                 rows of the matrices in assays.
-            colData (Union[pd.DataFrame, BiocFrame], optional): sample data, must be 
+            colData (Union[pd.DataFrame, BiocFrame], optional): sample data, must be
                 the same length as rows of the matrices in assays. Defaults to None.
-            metadata (MutableMapping, optional): experiment metadata describing the 
+            metadata (MutableMapping, optional): experiment metadata describing the
                 methods. Defaults to None.
         """
         super().__init__(assays, rowRanges, colData, metadata)
 
     def _validate_rows(self, rows: Optional[GenomicRanges]):
         """Internal method to validate feature information (`rowRanges`).
 
@@ -182,46 +182,46 @@
 
     def coverage(
         self, shift: int = 0, width: Optional[int] = None, weight: int = 1
     ) -> MutableMapping[str, np.ndarray]:
         """Calculate coverage for each chromosome.
 
         Args:
-            shift (int, optional): shifts all genomic positions by specified number 
+            shift (int, optional): shifts all genomic positions by specified number
                 of positions. Defaults to 0.
             width (int, optional): restrict the width of all chromosomes.
                 Defaults to None.
             weight (int, optional): weight to use. Defaults to 1.
 
         Returns:
-            MutableMapping[str, np.ndarray]: a dictionary containing chromosome names 
+            MutableMapping[str, np.ndarray]: a dictionary containing chromosome names
             as keys and the coverage vector as values.
         """
         return self.rowRanges.coverage(shift=shift, width=width, weight=weight)
 
     def nearest(
         self,
         query: Union[GenomicRanges, "RangeSummarizedExperiment"],
         ignoreStrand: bool = False,
     ) -> Optional[Sequence[Optional[int]]]:
-        """Search nearest positions, both upstream and downstream that overlap with 
+        """Search nearest positions, both upstream and downstream that overlap with
         each range in `query`.
 
         Args:
-            query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query intervals 
+            query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query intervals
                 to find nearest positions.
-            ignoreStrand (bool, optional): ignore strand during looksups? 
+            ignoreStrand (bool, optional): ignore strand during looksups?
                 Defaults to False.
 
         Raises:
-            TypeError: if `query` is not a `RangeSummarizedExperiment` 
+            TypeError: if `query` is not a `RangeSummarizedExperiment`
                 or `GenomicRanges`.
-            
+
         Returns:
-            Optional[Sequence[Optional[int]]]: List of possible hit indices 
+            Optional[Sequence[Optional[int]]]: List of possible hit indices
             for each interval in `query`. If there are no hits, returns None.
         """
 
         if not (
             isinstance(query, RangeSummarizedExperiment)
             or isinstance(query, GenomicRanges)
         ):
@@ -237,28 +237,28 @@
         return res.column("hits")
 
     def precede(
         self,
         query: Union[GenomicRanges, "RangeSummarizedExperiment"],
         ignoreStrand: bool = False,
     ) -> Optional[Sequence[Optional[int]]]:
-        """Search nearest positions, only downstream that overlap with 
+        """Search nearest positions, only downstream that overlap with
         each range in `query`.
 
         Args:
-            query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query intervals 
+            query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query intervals
                 to find nearest positions.
             ignoreStrand (bool, optional): ignore strand? Defaults to False.
 
         Raises:
-            TypeError: if query is not a `RangeSummarizedExperiment` or 
+            TypeError: if query is not a `RangeSummarizedExperiment` or
             `GenomicRanges`.
-        
+
         Returns:
-            Optional[Sequence[Optional[int]]]: List of possible hit indices 
+            Optional[Sequence[Optional[int]]]: List of possible hit indices
             for each interval in `query`. If there are no hits, returns None.
         """
 
         if not (
             isinstance(query, RangeSummarizedExperiment)
             or isinstance(query, GenomicRanges)
         ):
@@ -274,28 +274,28 @@
         return res.column("hits")
 
     def follow(
         self,
         query: Union[GenomicRanges, "RangeSummarizedExperiment"],
         ignoreStrand: bool = False,
     ) -> Optional[Sequence[Optional[int]]]:
-        """Search nearest positions, only upstream that overlap with the 
+        """Search nearest positions, only upstream that overlap with the
         each range in `query`.
 
         Args:
-            query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query intervals 
+            query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query intervals
                 to find nearest positions.
             ignoreStrand (bool, optional): ignore strand? Defaults to False.
 
         Raises:
-            TypeError: if query is not a `RangeSummarizedExperiment` or 
+            TypeError: if query is not a `RangeSummarizedExperiment` or
             `GenomicRanges`.
 
         Returns:
-            Optional[Sequence[Optional[int]]]: List of possible hit indices 
+            Optional[Sequence[Optional[int]]]: List of possible hit indices
             for each interval in `query`. If there are no hits, returns None.
         """
         if not (
             isinstance(query, RangeSummarizedExperiment)
             or isinstance(query, GenomicRanges)
         ):
             raise TypeError(
@@ -310,29 +310,29 @@
         return res.column("hits")
 
     def distanceToNearest(
         self,
         query: Union[GenomicRanges, "RangeSummarizedExperiment"],
         ignoreStrand: bool = False,
     ) -> Optional[Sequence[Optional[int]]]:
-        """Search nearest positions only downstream that overlap with the 
+        """Search nearest positions only downstream that overlap with the
         each genomics interval in `query`.
-        
+
         Technically same as `nearest` since we also return `distance` to the nearest match.
 
         Args:
-            query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query intervals 
+            query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query intervals
                 to find nearest positions.
             ignoreStrand (bool, optional): ignore strand? Defaults to False.
 
         Raises:
             TypeError: if query is not a `RangeSummarizedExperiment` or `GenomicRanges`.
 
         Returns:
-            Optional[Sequence[Optional[int]]]: List of possible hit indices 
+            Optional[Sequence[Optional[int]]]: List of possible hit indices
             for each interval in `query`. If there are no hits, returns None.
         """
         if not (
             isinstance(query, RangeSummarizedExperiment)
             or isinstance(query, GenomicRanges)
         ):
             raise TypeError(
@@ -361,45 +361,48 @@
         Args:
             width (int): width to flank by.
             start (bool, optional): only flank starts?. Defaults to True.
             both (bool, optional): both starts and ends?. Defaults to False.
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Returns:
-            RangeSummarizedExperiment: a new `RangeSummarizedExperiment` object 
+            RangeSummarizedExperiment: a new `RangeSummarizedExperiment` object
             with the flanked ranges.
         """
         new_ranges = self.rowRanges.flank(
             width=width, start=start, both=both, ignoreStrand=ignoreStrand
         )
 
         return RangeSummarizedExperiment(
             assays=self.assays,
             rowRanges=new_ranges,
             colData=self.colData,
             metadata=self.metadata,
         )
 
     def resize(
-        self, width: int, fix: str = "start", ignoreStrand: bool = False,
+        self,
+        width: int,
+        fix: str = "start",
+        ignoreStrand: bool = False,
     ) -> "RangeSummarizedExperiment":
-        """Resize `rowRanges` to the specified `width` where either the `start`, 
+        """Resize `rowRanges` to the specified `width` where either the `start`,
         `end`, or `center` is used as an anchor.
 
         Args:
             width (int): width to resize by.
-            fix (str, optional): fix positions by `start`, `end` or `center`. 
+            fix (str, optional): fix positions by `start`, `end` or `center`.
                 Defaults to "start".
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Raises:
             ValueError: parameter fix is neither `start`, `cetner`, or `end`.
 
         Returns:
-            RangeSummarizedExperiment: a new `RangeSummarizedExperiment` object 
+            RangeSummarizedExperiment: a new `RangeSummarizedExperiment` object
             with the resized ranges.
         """
         new_ranges = self.rowRanges.resize(
             width=width, fix=fix, ignoreStrand=ignoreStrand
         )
 
         return RangeSummarizedExperiment(
@@ -414,15 +417,15 @@
 
         shift can be be a negative parameter.
 
         Args:
             shift (int, optional): shift interval. Defaults to 0.
 
         Returns:
-            RangeSummarizedExperiment: a new `RangeSummarizedExperiment` 
+            RangeSummarizedExperiment: a new `RangeSummarizedExperiment`
             object with the shifted ranges.
         """
 
         if self.rowRanges is None:
             raise ValueError("rowRanges is None")
 
         new_ranges = self.rowRanges.shift(shift=shift)
@@ -436,21 +439,21 @@
 
     def promoters(
         self, upstream: int = 2000, downstream: int = 200
     ) -> "RangeSummarizedExperiment":
         """Extend `rowRanges` to promoter regions.
 
         Args:
-            upstream (int, optional): number of positions to extend 
+            upstream (int, optional): number of positions to extend
                 in the 5' direction . Defaults to 2000.
-            downstream (int, optional): number of positions to extend 
+            downstream (int, optional): number of positions to extend
                 in the 3' direction. Defaults to 200.
 
         Returns:
-            RangeSummarizedExperiment: a new `RangeSummarizedExperiment` 
+            RangeSummarizedExperiment: a new `RangeSummarizedExperiment`
             object with the extended ranges for promoter regions.
         """
         new_ranges = self.rowRanges.promoters(upstream=upstream, downstream=downstream)
 
         return RangeSummarizedExperiment(
             assays=self.assays,
             rowRanges=new_ranges,
@@ -465,19 +468,19 @@
         keepAllRanges: bool = False,
     ) -> "RangeSummarizedExperiment":
         """Restrict `rowRanges` to a given start and end positions.
 
         Args:
             start (int, optional): start position. Defaults to None.
             end (int, optional): end position. Defaults to None.
-            keepAllRanges (bool, optional): Keep intervals that do not 
+            keepAllRanges (bool, optional): Keep intervals that do not
                 overlap with start and end?. Defaults to False.
 
         Returns:
-            RangeSummarizedExperiment: a new `RangeSummarizedExperiment` 
+            RangeSummarizedExperiment: a new `RangeSummarizedExperiment`
             object with restricted intervals.
         """
         new_ranges = self.rowRanges.restrict(
             start=start, end=end, keepAllRanges=keepAllRanges
         )
 
         return RangeSummarizedExperiment(
@@ -502,15 +505,15 @@
             width (int, optional): relative end position. Defaults to None.
             end (int, optional): relative width of the interval. Defaults to None.
 
         Raises:
             ValueError: when parameters were set incorrectly or rowRanges is empty
 
         Returns:
-            RangeSummarizedExperiment:  a new `RangeSummarizedExperiment` 
+            RangeSummarizedExperiment:  a new `RangeSummarizedExperiment`
             object with narrow positions.
         """
         new_ranges = self.rowRanges.narrow(start=start, width=width, end=end)
 
         return RangeSummarizedExperiment(
             assays=self.assays,
             rowRanges=new_ranges,
@@ -526,30 +529,30 @@
         minOverlap: int = 1,
         ignoreStrand: bool = False,
     ) -> Optional["RangeSummarizedExperiment"]:
         """Find overlaps between subject (self) and query ranges.
 
         Args:
             query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query ranges.
-            queryType (str, optional): overlap query type, must be one of 
+            queryType (str, optional): overlap query type, must be one of
                 - "any": any overlap is good.
                 - "start": overlap at the beginning of the intervals.
                 - "end": must overlap at the end of the intervals.
-                - "within": fully contain the query interval. 
+                - "within": fully contain the query interval.
                 Defaults to any.
-            maxGap (int, optional): maximum gap allowed in the overlap. 
+            maxGap (int, optional): maximum gap allowed in the overlap.
                 Defaults to -1 (no gap allowed).
-            minOverlap (int, optional): minimum overlap with query. Defaults to 1. 
+            minOverlap (int, optional): minimum overlap with query. Defaults to 1.
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Raises:
             TypeError: if query is not a `RangeSummarizedExperiment` or `GenomicRanges`.
 
         Returns:
-            Optional["RangeSummarizedExperiment"]: A `RangeSummarizedExperiment` object 
+            Optional["RangeSummarizedExperiment"]: A `RangeSummarizedExperiment` object
             with the same length as query, containing hits to overlapping indices.
         """
 
         if not (
             isinstance(query, RangeSummarizedExperiment)
             or isinstance(query, GenomicRanges)
         ):
@@ -577,30 +580,30 @@
         minOverlap: int = 1,
         ignoreStrand: bool = False,
     ) -> Optional["RangeSummarizedExperiment"]:
         """Subset a `RangeSummarizedExperiment` by feature overlaps.
 
         Args:
             query (Union[GenomicRanges, "RangeSummarizedExperiment"]): query ranges.
-            queryType (str, optional): overlap query type, must be one of 
+            queryType (str, optional): overlap query type, must be one of
                 - "any": any overlap is good.
                 - "start": overlap at the beginning of the intervals.
                 - "end": must overlap at the end of the intervals.
-                - "within": fully contain the query interval. 
+                - "within": fully contain the query interval.
                 Defaults to any.
-            maxGap (int, optional): maximum gap allowed in the overlap. 
+            maxGap (int, optional): maximum gap allowed in the overlap.
                 Defaults to -1 (no gap allowed).
-            minOverlap (int, optional): minimum overlap with query. Defaults to 1. 
+            minOverlap (int, optional): minimum overlap with query. Defaults to 1.
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Raises:
             TypeError: if query is not a `RangeSummarizedExperiment` or `GenomicRanges`.
 
         Returns:
-            Optional["RangeSummarizedExperiment"]: new `RangeSummarizedExperiment` 
+            Optional["RangeSummarizedExperiment"]: new `RangeSummarizedExperiment`
             object. None if there are no indices to slice.
         """
 
         if not (
             isinstance(query, RangeSummarizedExperiment)
             or isinstance(query, GenomicRanges)
         ):
@@ -646,15 +649,15 @@
         """Sort `RangeSummarizedExperiment` by `rowRanges`.
 
         Args:
             decreasing (bool, optional): decreasing order?. Defaults to False.
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Returns:
-            "RangeSummarizedExperiment": a new sorted 
+            "RangeSummarizedExperiment": a new sorted
             `RangeSummarizedExperiment` object.
         """
         order = self.rowRanges._generic_order(ignoreStrand=ignoreStrand)
 
         if decreasing:
             order = order[::-1]
```

### Comparing `SummarizedExperiment-0.2.4/src/summarizedexperiment/SummarizedExperiment.py` & `SummarizedExperiment-0.2.5/src/summarizedexperiment/SummarizedExperiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Union, Tuple, Optional, Sequence, MutableMapping
-from biocframe import BiocFrame
-import pandas as pd
+from typing import MutableMapping, Optional, Sequence, Tuple, Union
+
 import numpy as np
+import pandas as pd
+from biocframe import BiocFrame
 from scipy import sparse as sp
 
 from .BaseSE import BaseSE
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
@@ -21,27 +22,27 @@
         assays: MutableMapping[str, Union[np.ndarray, sp.spmatrix]],
         rowData: Optional[Union[pd.DataFrame, BiocFrame]] = None,
         colData: Optional[Union[pd.DataFrame, BiocFrame]] = None,
         metadata: Optional[MutableMapping] = None,
     ) -> None:
         """Initialize a Summarized Experiment (SE).
 
-        SE follows the R/Bioconductor specification; rows are features, columns are 
+        SE follows the R/Bioconductor specification; rows are features, columns are
         samples.
 
         Args:
-            assays (MutableMapping[str, Union[np.ndarray, sp.spmatrix]]): dictionary 
-                of matrices, with assay names as keys and matrices represented as dense 
-                (numpy) or sparse (scipy) matrices. All matrices across assays must 
+            assays (MutableMapping[str, Union[np.ndarray, sp.spmatrix]]): dictionary
+                of matrices, with assay names as keys and matrices represented as dense
+                (numpy) or sparse (scipy) matrices. All matrices across assays must
                 have the same dimensions (number of rows, number of columns).
-            rowData (GenomicRanges, optional): features, must be the same length as 
+            rowData (GenomicRanges, optional): features, must be the same length as
                 rows of the matrices in assays. Defaults to None.
-            colData (Union[pd.DataFrame, BiocFrame], optional): sample data, must be 
+            colData (Union[pd.DataFrame, BiocFrame], optional): sample data, must be
                 the same length as rows of the matrices in assays. Defaults to None.
-            metadata (MutableMapping, optional): experiment metadata describing the 
+            metadata (MutableMapping, optional): experiment metadata describing the
                 methods. Defaults to None.
         """
         super().__init__(assays, rowData, colData, metadata)
 
     @property
     def rowData(self) -> Union[pd.DataFrame, BiocFrame]:
         """Get features.
```

### Comparing `SummarizedExperiment-0.2.4/src/summarizedexperiment/__init__.py` & `SummarizedExperiment-0.2.5/src/summarizedexperiment/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
 from .SummarizedExperiment import SummarizedExperiment
 from .RangeSummarizedExperiment import RangeSummarizedExperiment
+from .RangedSummarizedExperiment import RangedSummarizedExperiment
```

### Comparing `SummarizedExperiment-0.2.4/tests/test_RSE.py` & `SummarizedExperiment-0.2.5/tests/test_RSE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/tests/test_RSE_methods.py` & `SummarizedExperiment-0.2.5/tests/test_RSE_methods.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/tests/test_SE.py` & `SummarizedExperiment-0.2.5/tests/test_SE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/tests/test_SE_methods.py` & `SummarizedExperiment-0.2.5/tests/test_SE_methods.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.4/tox.ini` & `SummarizedExperiment-0.2.5/tox.ini`

 * *Files identical despite different names*

