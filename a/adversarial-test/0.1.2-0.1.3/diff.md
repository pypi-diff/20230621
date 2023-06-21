# Comparing `tmp/adversarial-test-0.1.2.tar.gz` & `tmp/adversarial-test-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adversarial-test-0.1.2.tar", last modified: Wed Jun 21 04:17:44 2023, max compression
+gzip compressed data, was "adversarial-test-0.1.3.tar", last modified: Wed Jun 21 04:21:39 2023, max compression
```

## Comparing `adversarial-test-0.1.2.tar` & `adversarial-test-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 04:17:44.554190 adversarial-test-0.1.2/
--rw-r--r--   0 lap14814   (501) staff       (20)      180 2023-06-21 04:17:44.553954 adversarial-test-0.1.2/PKG-INFO
--rw-r--r--   0 lap14814   (501) staff       (20)      697 2023-06-21 03:42:35.000000 adversarial-test-0.1.2/README.md
-drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 04:17:44.552767 adversarial-test-0.1.2/adversarial/
--rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-21 03:38:13.000000 adversarial-test-0.1.2/adversarial/__init__.py
--rw-r--r--   0 lap14814   (501) staff       (20)     2665 2023-06-21 03:38:13.000000 adversarial-test-0.1.2/adversarial/adversarial_test.py
-drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 04:17:44.553554 adversarial-test-0.1.2/adversarial_test.egg-info/
--rw-r--r--   0 lap14814   (501) staff       (20)      180 2023-06-21 04:17:44.000000 adversarial-test-0.1.2/adversarial_test.egg-info/PKG-INFO
--rw-r--r--   0 lap14814   (501) staff       (20)      322 2023-06-21 04:17:44.000000 adversarial-test-0.1.2/adversarial_test.egg-info/SOURCES.txt
--rw-r--r--   0 lap14814   (501) staff       (20)        1 2023-06-21 04:17:44.000000 adversarial-test-0.1.2/adversarial_test.egg-info/dependency_links.txt
--rw-r--r--   0 lap14814   (501) staff       (20)       35 2023-06-21 04:17:44.000000 adversarial-test-0.1.2/adversarial_test.egg-info/requires.txt
--rw-r--r--   0 lap14814   (501) staff       (20)       18 2023-06-21 04:17:44.000000 adversarial-test-0.1.2/adversarial_test.egg-info/top_level.txt
--rw-r--r--   0 lap14814   (501) staff       (20)       38 2023-06-21 04:17:44.554231 adversarial-test-0.1.2/setup.cfg
--rw-r--r--   0 lap14814   (501) staff       (20)      469 2023-06-21 04:17:41.000000 adversarial-test-0.1.2/setup.py
-drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 04:17:44.553770 adversarial-test-0.1.2/tests/
--rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-21 03:38:13.000000 adversarial-test-0.1.2/tests/__init__.py
--rw-r--r--   0 lap14814   (501) staff       (20)     3404 2023-06-21 03:38:13.000000 adversarial-test-0.1.2/tests/test_adversarial_test.py
+drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 04:21:39.066177 adversarial-test-0.1.3/
+-rw-r--r--   0 lap14814   (501) staff       (20)      918 2023-06-21 04:21:39.065937 adversarial-test-0.1.3/PKG-INFO
+-rw-r--r--   0 lap14814   (501) staff       (20)      697 2023-06-21 03:42:35.000000 adversarial-test-0.1.3/README.md
+drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 04:21:39.064669 adversarial-test-0.1.3/adversarial/
+-rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-21 03:38:13.000000 adversarial-test-0.1.3/adversarial/__init__.py
+-rw-r--r--   0 lap14814   (501) staff       (20)     2665 2023-06-21 03:38:13.000000 adversarial-test-0.1.3/adversarial/adversarial_test.py
+drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 04:21:39.065482 adversarial-test-0.1.3/adversarial_test.egg-info/
+-rw-r--r--   0 lap14814   (501) staff       (20)      918 2023-06-21 04:21:39.000000 adversarial-test-0.1.3/adversarial_test.egg-info/PKG-INFO
+-rw-r--r--   0 lap14814   (501) staff       (20)      322 2023-06-21 04:21:39.000000 adversarial-test-0.1.3/adversarial_test.egg-info/SOURCES.txt
+-rw-r--r--   0 lap14814   (501) staff       (20)        1 2023-06-21 04:21:39.000000 adversarial-test-0.1.3/adversarial_test.egg-info/dependency_links.txt
+-rw-r--r--   0 lap14814   (501) staff       (20)       35 2023-06-21 04:21:39.000000 adversarial-test-0.1.3/adversarial_test.egg-info/requires.txt
+-rw-r--r--   0 lap14814   (501) staff       (20)       18 2023-06-21 04:21:39.000000 adversarial-test-0.1.3/adversarial_test.egg-info/top_level.txt
+-rw-r--r--   0 lap14814   (501) staff       (20)       38 2023-06-21 04:21:39.066213 adversarial-test-0.1.3/setup.cfg
+-rw-r--r--   0 lap14814   (501) staff       (20)      725 2023-06-21 04:21:35.000000 adversarial-test-0.1.3/setup.py
+drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 04:21:39.065726 adversarial-test-0.1.3/tests/
+-rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-21 03:38:13.000000 adversarial-test-0.1.3/tests/__init__.py
+-rw-r--r--   0 lap14814   (501) staff       (20)     3404 2023-06-21 03:38:13.000000 adversarial-test-0.1.3/tests/test_adversarial_test.py
```

### Comparing `adversarial-test-0.1.2/README.md` & `adversarial-test-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `adversarial-test-0.1.2/adversarial/adversarial_test.py` & `adversarial-test-0.1.3/adversarial/adversarial_test.py`

 * *Files identical despite different names*

### Comparing `adversarial-test-0.1.2/tests/test_adversarial_test.py` & `adversarial-test-0.1.3/tests/test_adversarial_test.py`

 * *Files identical despite different names*

