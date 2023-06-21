# Comparing `tmp/design_kgex-0.0.6.tar.gz` & `tmp/design_kgex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design_kgex-0.0.6.tar", last modified: Wed Jun 21 04:51:35 2023, max compression
+gzip compressed data, was "design_kgex-0.1.1.tar", last modified: Wed Jun 21 04:55:48 2023, max compression
```

## Comparing `design_kgex-0.0.6.tar` & `design_kgex-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 04:51:35.872718 design_kgex-0.0.6/
--rw-rw-rw-   0        0        0     1134 2023-06-18 07:04:17.000000 design_kgex-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       85 2023-06-19 19:22:36.000000 design_kgex-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      295 2023-06-21 04:51:35.870000 design_kgex-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5139 2023-06-19 22:33:14.000000 design_kgex-0.0.6/README.md
--rw-rw-rw-   0        0        0       82 2023-06-19 10:38:09.000000 design_kgex-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 04:51:35.872897 design_kgex-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-06-21 04:50:22.000000 design_kgex-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 04:51:35.748405 design_kgex-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 04:51:35.838888 design_kgex-0.0.6/src/design_kgex/
--rw-rw-rw-   0        0        0        0 2023-06-18 03:55:58.000000 design_kgex-0.0.6/src/design_kgex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 04:51:35.866540 design_kgex-0.0.6/src/design_kgex/__pycache__/
--rw-rw-rw-   0        0        0     4962 2023-06-21 03:32:51.000000 design_kgex-0.0.6/src/design_kgex/__pycache__/design_knowledge.cpython-39.pyc
--rw-rw-rw-   0        0        0     4299 2023-06-21 03:32:58.000000 design_kgex-0.0.6/src/design_kgex/__pycache__/patent_text.cpython-39.pyc
--rw-rw-rw-   0        0        0     5415 2023-06-21 03:37:47.000000 design_kgex-0.0.6/src/design_kgex/design_knowledge.py
--rw-rw-rw-   0        0        0     5676 2023-06-21 04:38:38.000000 design_kgex-0.0.6/src/design_kgex/patent_text.py
--rw-rw-rw-   0        0        0    15722 2023-06-19 20:46:57.000000 design_kgex-0.0.6/src/design_kgex/supplementary.pkl
-drwxrwxrwx   0        0        0        0 2023-06-21 04:51:35.858698 design_kgex-0.0.6/src/design_kgex.egg-info/
--rw-rw-rw-   0        0        0      295 2023-06-21 04:51:35.000000 design_kgex-0.0.6/src/design_kgex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-06-21 04:51:35.000000 design_kgex-0.0.6/src/design_kgex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 04:51:35.000000 design_kgex-0.0.6/src/design_kgex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-06-21 04:51:35.000000 design_kgex-0.0.6/src/design_kgex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-21 04:51:35.000000 design_kgex-0.0.6/src/design_kgex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 04:55:48.139413 design_kgex-0.1.1/
+-rw-rw-rw-   0        0        0     1134 2023-06-18 07:04:17.000000 design_kgex-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-06-19 19:22:36.000000 design_kgex-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      295 2023-06-21 04:55:48.134198 design_kgex-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5139 2023-06-19 22:33:14.000000 design_kgex-0.1.1/README.md
+-rw-rw-rw-   0        0        0       82 2023-06-19 10:38:09.000000 design_kgex-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 04:55:48.140410 design_kgex-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      691 2023-06-21 04:55:27.000000 design_kgex-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:55:47.981127 design_kgex-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:55:48.077491 design_kgex-0.1.1/src/design_kgex/
+-rw-rw-rw-   0        0        0        0 2023-06-18 03:55:58.000000 design_kgex-0.1.1/src/design_kgex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:55:48.129527 design_kgex-0.1.1/src/design_kgex/__pycache__/
+-rw-rw-rw-   0        0        0     4962 2023-06-21 03:32:51.000000 design_kgex-0.1.1/src/design_kgex/__pycache__/design_knowledge.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4299 2023-06-21 03:32:58.000000 design_kgex-0.1.1/src/design_kgex/__pycache__/patent_text.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5415 2023-06-21 03:37:47.000000 design_kgex-0.1.1/src/design_kgex/design_knowledge.py
+-rw-rw-rw-   0        0        0     5676 2023-06-21 04:38:38.000000 design_kgex-0.1.1/src/design_kgex/patent_text.py
+-rw-rw-rw-   0        0        0    15722 2023-06-19 20:46:57.000000 design_kgex-0.1.1/src/design_kgex/supplementary.pkl
+drwxrwxrwx   0        0        0        0 2023-06-21 04:55:48.114999 design_kgex-0.1.1/src/design_kgex.egg-info/
+-rw-rw-rw-   0        0        0      295 2023-06-21 04:55:47.000000 design_kgex-0.1.1/src/design_kgex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-06-21 04:55:47.000000 design_kgex-0.1.1/src/design_kgex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 04:55:47.000000 design_kgex-0.1.1/src/design_kgex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-06-21 04:55:47.000000 design_kgex-0.1.1/src/design_kgex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 04:55:47.000000 design_kgex-0.1.1/src/design_kgex.egg-info/top_level.txt
```

### Comparing `design_kgex-0.0.6/LICENSE` & `design_kgex-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.6/README.md` & `design_kgex-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.6/setup.py` & `design_kgex-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='design_kgex',
-    version='0.0.6',
+    version='0.1.1',
     author='L. Siddharth',
     author_email='siddharthl.iitrpr.sutd@gmail.com',
     description='Extracting Design Knowledge from Patent Text',
     license='2023 Data-Driven Innovation Lab, Singapore University of Technology and Design',
     install_requires=[
         'requests',
         'importlib-metadata; python_version == "3.8"',
         'spacy', 
-        'claucy',
         'en_core_web_sm',
         'en_core_web_trf',
-        'spacy-transformers',
         'beautifulsoup4',
 	'patool'
     ],
     package_dir = {"": "src"},
     packages=find_namespace_packages(where='src'),
     include_package_data=True
 )
```

### Comparing `design_kgex-0.0.6/src/design_kgex/__pycache__/design_knowledge.cpython-39.pyc` & `design_kgex-0.1.1/src/design_kgex/__pycache__/design_knowledge.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.6/src/design_kgex/__pycache__/patent_text.cpython-39.pyc` & `design_kgex-0.1.1/src/design_kgex/__pycache__/patent_text.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.6/src/design_kgex/design_knowledge.py` & `design_kgex-0.1.1/src/design_kgex/design_knowledge.py`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.6/src/design_kgex/patent_text.py` & `design_kgex-0.1.1/src/design_kgex/patent_text.py`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.6/src/design_kgex/supplementary.pkl` & `design_kgex-0.1.1/src/design_kgex/supplementary.pkl`

 * *Files identical despite different names*

