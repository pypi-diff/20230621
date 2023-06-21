# Comparing `tmp/endorpysetup-1.2.6.tar.gz` & `tmp/endorpysetup-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endorpysetup-1.2.6.tar", last modified: Wed Jun 21 14:01:48 2023, max compression
+gzip compressed data, was "endorpysetup-1.2.7.tar", last modified: Wed Jun 21 14:24:49 2023, max compression
```

## Comparing `endorpysetup-1.2.6.tar` & `endorpysetup-1.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 nareshdevasani   (501) staff       (20)        0 2023-06-21 14:01:48.893619 endorpysetup-1.2.6/
--rw-r--r--   0 nareshdevasani   (501) staff       (20)      843 2023-06-21 14:01:48.893486 endorpysetup-1.2.6/PKG-INFO
--rw-r--r--   0 nareshdevasani   (501) staff       (20)       55 2022-11-29 10:54:42.000000 endorpysetup-1.2.6/README.md
-drwxr-xr-x   0 nareshdevasani   (501) staff       (20)        0 2023-06-21 14:01:48.893313 endorpysetup-1.2.6/endorpysetup.egg-info/
--rw-r--r--   0 nareshdevasani   (501) staff       (20)      843 2023-06-21 14:01:48.000000 endorpysetup-1.2.6/endorpysetup.egg-info/PKG-INFO
--rw-r--r--   0 nareshdevasani   (501) staff       (20)      197 2023-06-21 14:01:48.000000 endorpysetup-1.2.6/endorpysetup.egg-info/SOURCES.txt
--rw-r--r--   0 nareshdevasani   (501) staff       (20)        1 2023-06-21 14:01:48.000000 endorpysetup-1.2.6/endorpysetup.egg-info/dependency_links.txt
--rw-r--r--   0 nareshdevasani   (501) staff       (20)       63 2023-06-21 14:01:48.000000 endorpysetup-1.2.6/endorpysetup.egg-info/requires.txt
--rw-r--r--   0 nareshdevasani   (501) staff       (20)        1 2023-06-21 14:01:48.000000 endorpysetup-1.2.6/endorpysetup.egg-info/top_level.txt
--rw-r--r--   0 nareshdevasani   (501) staff       (20)       38 2023-06-21 14:01:48.893658 endorpysetup-1.2.6/setup.cfg
--rw-r--r--   0 nareshdevasani   (501) staff       (20)     1156 2023-06-21 13:56:14.000000 endorpysetup-1.2.6/setup.py
+drwxr-xr-x   0 nareshdevasani   (501) staff       (20)        0 2023-06-21 14:24:49.996515 endorpysetup-1.2.7/
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)      854 2023-06-21 14:24:49.996400 endorpysetup-1.2.7/PKG-INFO
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)       55 2022-11-29 10:54:42.000000 endorpysetup-1.2.7/README.md
+drwxr-xr-x   0 nareshdevasani   (501) staff       (20)        0 2023-06-21 14:24:49.996242 endorpysetup-1.2.7/endorpysetup.egg-info/
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)      854 2023-06-21 14:24:49.000000 endorpysetup-1.2.7/endorpysetup.egg-info/PKG-INFO
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)      197 2023-06-21 14:24:49.000000 endorpysetup-1.2.7/endorpysetup.egg-info/SOURCES.txt
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)        1 2023-06-21 14:24:49.000000 endorpysetup-1.2.7/endorpysetup.egg-info/dependency_links.txt
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)       55 2023-06-21 14:24:49.000000 endorpysetup-1.2.7/endorpysetup.egg-info/requires.txt
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)        1 2023-06-21 14:24:49.000000 endorpysetup-1.2.7/endorpysetup.egg-info/top_level.txt
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)       38 2023-06-21 14:24:49.996548 endorpysetup-1.2.7/setup.cfg
+-rw-r--r--   0 nareshdevasani   (501) staff       (20)     1149 2023-06-21 14:24:40.000000 endorpysetup-1.2.7/setup.py
```

### Comparing `endorpysetup-1.2.6/PKG-INFO` & `endorpysetup-1.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: endorpysetup
-Version: 1.2.6
-Summary: Having non-existing package under extras
+Version: 1.2.7
+Summary: Having non-existing package under normal dependencies - install_requires
 Home-page: http://github.com/endorlabs/python-deps
 Author: Endor labs Contributors
 Author-email: infolabs@goog.com
 License: Simplified BSD
 Keywords: endor tree fullmapping dict demo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -14,8 +14,7 @@
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: fido
```

### Comparing `endorpysetup-1.2.6/endorpysetup.egg-info/PKG-INFO` & `endorpysetup-1.2.7/endorpysetup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: endorpysetup
-Version: 1.2.6
-Summary: Having non-existing package under extras
+Version: 1.2.7
+Summary: Having non-existing package under normal dependencies - install_requires
 Home-page: http://github.com/endorlabs/python-deps
 Author: Endor labs Contributors
 Author-email: infolabs@goog.com
 License: Simplified BSD
 Keywords: endor tree fullmapping dict demo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -14,8 +14,7 @@
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: fido
```

### Comparing `endorpysetup-1.2.6/setup.py` & `endorpysetup-1.2.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
-version = '1.2.6'
-shortdesc = "Having non-existing package under extras"
+version = '1.2.7'
+shortdesc = "Having non-existing package under normal dependencies - install_requires"
 
 setup(
     name='endorpysetup',
     version=version,
     description=shortdesc,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
@@ -24,14 +24,12 @@
     author='Endor labs Contributors',
     author_email='infolabs@goog.com',
     url='http://github.com/endorlabs/python-deps',
     license='Simplified BSD',
     install_requires=[
         'odict==1.9.0',
         'plumber>=1.5,<1.7',
+        'non-existing-pkg >= 4.2.1'
     ],
-    extras_require={
-        'fido': ['non-existing-pkg >= 4.2.1'],
-    },
     test_suite='endor.tests.test_suite',
     py_modules=[]
 )
```

