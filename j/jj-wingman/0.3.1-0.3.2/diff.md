# Comparing `tmp/jj_wingman-0.3.1.tar.gz` & `tmp/jj_wingman-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj_wingman-0.3.1.tar", last modified: Wed Jun 21 18:30:00 2023, max compression
+gzip compressed data, was "jj_wingman-0.3.2.tar", last modified: Wed Jun 21 18:30:56 2023, max compression
```

## Comparing `jj_wingman-0.3.1.tar` & `jj_wingman-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:30:00.066430 jj_wingman-0.3.1/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.3.1/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)    15257 2023-06-21 18:30:00.066430 jj_wingman-0.3.1/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)    13561 2023-06-21 18:20:33.000000 jj_wingman-0.3.1/README.md
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:30:00.066430 jj_wingman-0.3.1/jj_wingman.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)    15257 2023-06-21 18:30:00.000000 jj_wingman-0.3.1/jj_wingman.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-06-21 18:30:00.000000 jj_wingman-0.3.1/jj_wingman.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-06-21 18:30:00.000000 jj_wingman-0.3.1/jj_wingman.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-06-21 18:30:00.000000 jj_wingman-0.3.1/jj_wingman.egg-info/entry_points.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-06-21 18:30:00.000000 jj_wingman-0.3.1/jj_wingman.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-06-21 18:30:00.000000 jj_wingman-0.3.1/jj_wingman.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-06-21 18:29:56.000000 jj_wingman-0.3.1/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-06-21 18:30:00.066430 jj_wingman-0.3.1/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.3.1/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:30:00.066430 jj_wingman-0.3.1/test/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3917 2023-05-29 12:52:26.000000 jj_wingman-0.3.1/test/test_replay_buffer.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:30:00.066430 jj_wingman-0.3.1/wingman/
--rw-rw-r--   0 jet       (1000) jet       (1000)      218 2023-06-02 11:46:07.000000 jj_wingman-0.3.1/wingman/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.3.1/wingman/cli_scripts.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      306 2023-06-21 18:19:17.000000 jj_wingman-0.3.1/wingman/config.yaml
--rw-rw-r--   0 jet       (1000) jet       (1000)    10283 2023-06-02 11:46:40.000000 jj_wingman-0.3.1/wingman/neural_blocks.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1006 2023-06-21 18:26:32.000000 jj_wingman-0.3.1/wingman/print_utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.3.1/wingman/replay_buffer.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-06-01 08:57:08.000000 jj_wingman-0.3.1/wingman/utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15928 2023-06-21 18:29:43.000000 jj_wingman-0.3.1/wingman/wingman.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:30:56.153945 jj_wingman-0.3.2/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.3.2/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15257 2023-06-21 18:30:56.153945 jj_wingman-0.3.2/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)    13561 2023-06-21 18:20:33.000000 jj_wingman-0.3.2/README.md
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:30:56.149945 jj_wingman-0.3.2/jj_wingman.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15257 2023-06-21 18:30:56.000000 jj_wingman-0.3.2/jj_wingman.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-06-21 18:30:56.000000 jj_wingman-0.3.2/jj_wingman.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-06-21 18:30:56.000000 jj_wingman-0.3.2/jj_wingman.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-06-21 18:30:56.000000 jj_wingman-0.3.2/jj_wingman.egg-info/entry_points.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-06-21 18:30:56.000000 jj_wingman-0.3.2/jj_wingman.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-06-21 18:30:56.000000 jj_wingman-0.3.2/jj_wingman.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-06-21 18:30:41.000000 jj_wingman-0.3.2/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-06-21 18:30:56.153945 jj_wingman-0.3.2/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.3.2/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:30:56.149945 jj_wingman-0.3.2/test/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3917 2023-05-29 12:52:26.000000 jj_wingman-0.3.2/test/test_replay_buffer.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:30:56.153945 jj_wingman-0.3.2/wingman/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      218 2023-06-02 11:46:07.000000 jj_wingman-0.3.2/wingman/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.3.2/wingman/cli_scripts.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      306 2023-06-21 18:19:17.000000 jj_wingman-0.3.2/wingman/config.yaml
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10283 2023-06-02 11:46:40.000000 jj_wingman-0.3.2/wingman/neural_blocks.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1006 2023-06-21 18:30:37.000000 jj_wingman-0.3.2/wingman/print_utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.3.2/wingman/replay_buffer.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-06-01 08:57:08.000000 jj_wingman-0.3.2/wingman/utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15928 2023-06-21 18:29:43.000000 jj_wingman-0.3.2/wingman/wingman.py
```

### Comparing `jj_wingman-0.3.1/LICENSE.txt` & `jj_wingman-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.1/PKG-INFO` & `jj_wingman-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.3.1
+Version: 0.3.2
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `jj_wingman-0.3.1/README.md` & `jj_wingman-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.1/jj_wingman.egg-info/PKG-INFO` & `jj_wingman-0.3.2/jj_wingman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj-wingman
-Version: 0.3.1
+Version: 0.3.2
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `jj_wingman-0.3.1/pyproject.toml` & `jj_wingman-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jj_wingman"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "Wingman library for AI projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jj_wingman-0.3.1/test/test_replay_buffer.py` & `jj_wingman-0.3.2/test/test_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.1/wingman/cli_scripts.py` & `jj_wingman-0.3.2/wingman/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.1/wingman/neural_blocks.py` & `jj_wingman-0.3.2/wingman/neural_blocks.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.1/wingman/print_utils.py` & `jj_wingman-0.3.2/wingman/print_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,9 +41,9 @@
         log_file (str): a target path to save the log file if any
     """
     print(f"{log_flag}: {x}")
 
     if not log_file:
         return
 
-    with open(log_file, "x") as f:
+    with open(log_file, "a") as f:
         f.write(f"{x}\n")
```

### Comparing `jj_wingman-0.3.1/wingman/replay_buffer.py` & `jj_wingman-0.3.2/wingman/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.1/wingman/utils.py` & `jj_wingman-0.3.2/wingman/utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.1/wingman/wingman.py` & `jj_wingman-0.3.2/wingman/wingman.py`

 * *Files identical despite different names*

