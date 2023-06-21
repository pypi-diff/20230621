# Comparing `tmp/jj_wingman-0.3.3.tar.gz` & `tmp/jj_wingman-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj_wingman-0.3.3.tar", last modified: Wed Jun 21 18:33:30 2023, max compression
+gzip compressed data, was "jj_wingman-0.3.4.tar", last modified: Wed Jun 21 18:43:52 2023, max compression
```

## Comparing `jj_wingman-0.3.3.tar` & `jj_wingman-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:33:30.036271 jj_wingman-0.3.3/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.3.3/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)    15257 2023-06-21 18:33:30.036271 jj_wingman-0.3.3/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)    13561 2023-06-21 18:20:33.000000 jj_wingman-0.3.3/README.md
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:33:30.036271 jj_wingman-0.3.3/jj_wingman.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)    15257 2023-06-21 18:33:30.000000 jj_wingman-0.3.3/jj_wingman.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-06-21 18:33:30.000000 jj_wingman-0.3.3/jj_wingman.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-06-21 18:33:30.000000 jj_wingman-0.3.3/jj_wingman.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-06-21 18:33:30.000000 jj_wingman-0.3.3/jj_wingman.egg-info/entry_points.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-06-21 18:33:30.000000 jj_wingman-0.3.3/jj_wingman.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-06-21 18:33:30.000000 jj_wingman-0.3.3/jj_wingman.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-06-21 18:33:26.000000 jj_wingman-0.3.3/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-06-21 18:33:30.036271 jj_wingman-0.3.3/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.3.3/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:33:30.036271 jj_wingman-0.3.3/test/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3917 2023-05-29 12:52:26.000000 jj_wingman-0.3.3/test/test_replay_buffer.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:33:30.036271 jj_wingman-0.3.3/wingman/
--rw-rw-r--   0 jet       (1000) jet       (1000)      218 2023-06-02 11:46:07.000000 jj_wingman-0.3.3/wingman/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.3.3/wingman/cli_scripts.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      306 2023-06-21 18:19:17.000000 jj_wingman-0.3.3/wingman/config.yaml
--rw-rw-r--   0 jet       (1000) jet       (1000)    10283 2023-06-02 11:46:40.000000 jj_wingman-0.3.3/wingman/neural_blocks.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1006 2023-06-21 18:30:37.000000 jj_wingman-0.3.3/wingman/print_utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.3.3/wingman/replay_buffer.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-06-01 08:57:08.000000 jj_wingman-0.3.3/wingman/utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15839 2023-06-21 18:33:22.000000 jj_wingman-0.3.3/wingman/wingman.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:43:52.988161 jj_wingman-0.3.4/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.3.4/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15275 2023-06-21 18:43:52.988161 jj_wingman-0.3.4/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)    13579 2023-06-21 18:39:48.000000 jj_wingman-0.3.4/README.md
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:43:52.984161 jj_wingman-0.3.4/jj_wingman.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15275 2023-06-21 18:43:52.000000 jj_wingman-0.3.4/jj_wingman.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-06-21 18:43:52.000000 jj_wingman-0.3.4/jj_wingman.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-06-21 18:43:52.000000 jj_wingman-0.3.4/jj_wingman.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-06-21 18:43:52.000000 jj_wingman-0.3.4/jj_wingman.egg-info/entry_points.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-06-21 18:43:52.000000 jj_wingman-0.3.4/jj_wingman.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-06-21 18:43:52.000000 jj_wingman-0.3.4/jj_wingman.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-06-21 18:43:49.000000 jj_wingman-0.3.4/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-06-21 18:43:52.988161 jj_wingman-0.3.4/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.3.4/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:43:52.988161 jj_wingman-0.3.4/test/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3917 2023-05-29 12:52:26.000000 jj_wingman-0.3.4/test/test_replay_buffer.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-21 18:43:52.988161 jj_wingman-0.3.4/wingman/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      218 2023-06-02 11:46:07.000000 jj_wingman-0.3.4/wingman/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.3.4/wingman/cli_scripts.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      306 2023-06-21 18:19:17.000000 jj_wingman-0.3.4/wingman/config.yaml
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10283 2023-06-02 11:46:40.000000 jj_wingman-0.3.4/wingman/neural_blocks.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1066 2023-06-21 18:43:42.000000 jj_wingman-0.3.4/wingman/print_utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.3.4/wingman/replay_buffer.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-06-01 08:57:08.000000 jj_wingman-0.3.4/wingman/utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15817 2023-06-21 18:43:26.000000 jj_wingman-0.3.4/wingman/wingman.py
```

### Comparing `jj_wingman-0.3.3/LICENSE.txt` & `jj_wingman-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.3/PKG-INFO` & `jj_wingman-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.3.3
+Version: 0.3.4
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -74,14 +74,15 @@
 ```yaml
 # wingman required params
 debug: false
 
 weights_directory: 'weights'
 version_number: null
 mark_number: 0
+log_status: false
 
 increment: true
 logging_interval: 10
 max_skips: 5
 greater_than: 0.0
 
 wandb: false
```

### Comparing `jj_wingman-0.3.3/README.md` & `jj_wingman-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 ```yaml
 # wingman required params
 debug: false
 
 weights_directory: 'weights'
 version_number: null
 mark_number: 0
+log_status: false
 
 increment: true
 logging_interval: 10
 max_skips: 5
 greater_than: 0.0
 
 wandb: false
```

### Comparing `jj_wingman-0.3.3/jj_wingman.egg-info/PKG-INFO` & `jj_wingman-0.3.4/jj_wingman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj-wingman
-Version: 0.3.3
+Version: 0.3.4
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -74,14 +74,15 @@
 ```yaml
 # wingman required params
 debug: false
 
 weights_directory: 'weights'
 version_number: null
 mark_number: 0
+log_status: false
 
 increment: true
 logging_interval: 10
 max_skips: 5
 greater_than: 0.0
 
 wandb: false
```

### Comparing `jj_wingman-0.3.3/pyproject.toml` & `jj_wingman-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jj_wingman"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "Wingman library for AI projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jj_wingman-0.3.3/test/test_replay_buffer.py` & `jj_wingman-0.3.4/test/test_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.3/wingman/cli_scripts.py` & `jj_wingman-0.3.4/wingman/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.3/wingman/neural_blocks.py` & `jj_wingman-0.3.4/wingman/neural_blocks.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.3/wingman/print_utils.py` & `jj_wingman-0.3.4/wingman/print_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """For fancy printing in Wingman."""
 from __future__ import annotations
 
+import re
 from typing import Any
 
 # colour list
 c_colors = {
     "HEADER": "\033[95m",
     "OKBLUE": "\033[94m",
     "OKCYAN": "\033[96m",
@@ -42,8 +43,9 @@
     """
     print(f"{log_flag}: {x}")
 
     if not log_file:
         return
 
     with open(log_file, "a") as f:
-        f.write(f"{x}\n")
+        f.write(re.sub(r"\[[0-9;]+[a-zA-Z]", " ", x))
+        f.write("\n")
```

### Comparing `jj_wingman-0.3.3/wingman/replay_buffer.py` & `jj_wingman-0.3.4/wingman/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.3/wingman/utils.py` & `jj_wingman-0.3.4/wingman/utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.3/wingman/wingman.py` & `jj_wingman-0.3.4/wingman/wingman.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,15 @@
             self.log_file = os.path.join(
                 self.version_directory,
                 "log.txt",
             )
 
         wm_print("--------------𓆩𓆪--------------")
         wm_print(f"Using device {cstr(self.device, 'HEADER')}")
-        wm_print(
-            f"Saving weights to {cstr(self.version_directory, 'HEADER')}..."
-        )
+        wm_print(f"Saving weights to {cstr(self.version_directory, 'HEADER')}...")
 
         # check to record that we're in a new training session
         self.fresh_directory = False
         if not os.path.isdir(self.version_directory):
             self.fresh_directory = True
             wm_print(
                 cstr(
```

