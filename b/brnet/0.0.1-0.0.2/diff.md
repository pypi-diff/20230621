# Comparing `tmp/brnet-0.0.1.tar.gz` & `tmp/brnet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brnet-0.0.1.tar", last modified: Wed Jun 21 17:14:01 2023, max compression
+gzip compressed data, was "brnet-0.0.2.tar", last modified: Wed Jun 21 20:46:55 2023, max compression
```

## Comparing `brnet-0.0.1.tar` & `brnet-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.176925 brnet-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.172925 brnet-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 17:13:48.000000 brnet-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.172925 brnet-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-21 17:13:48.000000 brnet-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-21 17:13:48.000000 brnet-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 17:13:48.000000 brnet-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 17:13:48.000000 brnet-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 17:13:48.000000 brnet-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-21 17:14:01.176925 brnet-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-21 17:13:48.000000 brnet-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-21 17:13:48.000000 brnet-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.172925 brnet-0.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:13:48.000000 brnet-0.0.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-21 17:13:48.000000 brnet-0.0.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:13:48.000000 brnet-0.0.1/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 17:13:48.000000 brnet-0.0.1/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:14:01.176925 brnet-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.172925 brnet-0.0.1/sh/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 17:13:48.000000 brnet-0.0.1/sh/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-21 17:13:48.000000 brnet-0.0.1/sh/brnet
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 17:13:48.000000 brnet-0.0.1/sh/pidp11.sh.diff
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-21 17:13:48.000000 brnet-0.0.1/sh/wait_for_if
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.172925 brnet-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.176925 brnet-0.0.1/src/brnet/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 17:13:48.000000 brnet-0.0.1/src/brnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-06-21 17:13:48.000000 brnet-0.0.1/src/brnet/bridger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-21 17:13:48.000000 brnet-0.0.1/src/brnet/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 17:13:48.000000 brnet-0.0.1/src/brnet/external.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.176925 brnet-0.0.1/src/brnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-21 17:14:01.000000 brnet-0.0.1/src/brnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 17:14:01.000000 brnet-0.0.1/src/brnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:14:01.000000 brnet-0.0.1/src/brnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 17:14:01.000000 brnet-0.0.1/src/brnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 17:14:01.000000 brnet-0.0.1/src/brnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:14:01.176925 brnet-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:13:48.000000 brnet-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 17:13:48.000000 brnet-0.0.1/tests/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 17:13:48.000000 brnet-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 20:46:45.000000 brnet-0.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-21 20:46:45.000000 brnet-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-21 20:46:45.000000 brnet-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 20:46:45.000000 brnet-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 20:46:45.000000 brnet-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 20:46:45.000000 brnet-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-21 20:46:55.748987 brnet-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-21 20:46:45.000000 brnet-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-21 20:46:45.000000 brnet-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:46:45.000000 brnet-0.0.2/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-21 20:46:45.000000 brnet-0.0.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:45.000000 brnet-0.0.2/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 20:46:45.000000 brnet-0.0.2/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:46:55.748987 brnet-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/sh/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 20:46:45.000000 brnet-0.0.2/sh/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-21 20:46:45.000000 brnet-0.0.2/sh/brnet
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 20:46:45.000000 brnet-0.0.2/sh/pidp11.sh.diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-21 20:46:45.000000 brnet-0.0.2/sh/wait_for_if
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.744987 brnet-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/src/brnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 20:46:45.000000 brnet-0.0.2/src/brnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-06-21 20:46:45.000000 brnet-0.0.2/src/brnet/bridger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-21 20:46:45.000000 brnet-0.0.2/src/brnet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 20:46:45.000000 brnet-0.0.2/src/brnet/external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/src/brnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:45.000000 brnet-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 20:46:45.000000 brnet-0.0.2/tests/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 20:46:45.000000 brnet-0.0.2/tox.ini
```

### Comparing `brnet-0.0.1/.github/workflows/ci.yaml` & `brnet-0.0.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/.gitignore` & `brnet-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/LICENSE` & `brnet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/Makefile` & `brnet-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/PKG-INFO` & `brnet-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `brnet-0.0.1/README.md` & `brnet-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/pyproject.toml` & `brnet-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/requirements/dev.txt` & `brnet-0.0.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/sh/README.md` & `brnet-0.0.2/sh/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/sh/brnet` & `brnet-0.0.2/sh/brnet`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/src/brnet/bridger.py` & `brnet-0.0.2/src/brnet/bridger.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/src/brnet/cli.py` & `brnet-0.0.2/src/brnet/cli.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/src/brnet/external.py` & `brnet-0.0.2/src/brnet/external.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/src/brnet.egg-info/PKG-INFO` & `brnet-0.0.2/src/brnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `brnet-0.0.1/src/brnet.egg-info/SOURCES.txt` & `brnet-0.0.2/src/brnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brnet-0.0.1/tox.ini` & `brnet-0.0.2/tox.ini`

 * *Files identical despite different names*

