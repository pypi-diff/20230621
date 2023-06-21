# Comparing `tmp/amplitude-data-wrapper-0.4.4.tar.gz` & `tmp/amplitude-data-wrapper-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplitude-data-wrapper-0.4.4.tar", last modified: Wed Jun 21 20:53:31 2023, max compression
+gzip compressed data, was "amplitude-data-wrapper-0.4.5.tar", last modified: Wed Jun 21 20:57:31 2023, max compression
```

## Comparing `amplitude-data-wrapper-0.4.4.tar` & `amplitude-data-wrapper-0.4.5.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:53:31.632546 amplitude-data-wrapper-0.4.4/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      121 2023-06-21 20:49:06.000000 amplitude-data-wrapper-0.4.4/.gitignore
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.4/CODEOWNERS
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.4/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      878 2023-06-21 19:20:48.000000 amplitude-data-wrapper-0.4.4/Makefile
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5901 2023-06-21 20:53:31.631907 amplitude-data-wrapper-0.4.4/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4278 2023-06-02 19:23:15.000000 amplitude-data-wrapper-0.4.4/README.md
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2175 2023-06-21 20:38:20.000000 amplitude-data-wrapper-0.4.4/example.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      809 2023-06-21 20:53:03.000000 amplitude-data-wrapper-0.4.4/pyproject.toml
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:53:31.616879 amplitude-data-wrapper-0.4.4/requirements/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3391 2023-06-21 19:22:04.000000 amplitude-data-wrapper-0.4.4/requirements/dev.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      438 2023-06-21 19:21:45.000000 amplitude-data-wrapper-0.4.4/requirements/main.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-06-21 20:53:31.632711 amplitude-data-wrapper-0.4.4/setup.cfg
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:53:31.609214 amplitude-data-wrapper-0.4.4/src/
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:53:31.619448 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:08:45.000000 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper/analytics_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:53:31.630042 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5901 2023-06-21 20:53:31.000000 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      473 2023-06-21 20:53:31.000000 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-21 20:53:31.000000 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       75 2023-06-21 20:53:31.000000 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper.egg-info/requires.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       32 2023-06-21 20:53:31.000000 amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:53:31.631003 amplitude-data-wrapper-0.4.4/src/examples/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2175 2023-06-21 20:38:37.000000 amplitude-data-wrapper-0.4.4/src/examples/example.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:57:31.774762 amplitude-data-wrapper-0.4.5/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      121 2023-06-21 20:49:06.000000 amplitude-data-wrapper-0.4.5/.gitignore
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.5/CODEOWNERS
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.5/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      878 2023-06-21 19:20:48.000000 amplitude-data-wrapper-0.4.5/Makefile
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5901 2023-06-21 20:57:31.773836 amplitude-data-wrapper-0.4.5/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4278 2023-06-02 19:23:15.000000 amplitude-data-wrapper-0.4.5/README.md
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2175 2023-06-21 20:38:20.000000 amplitude-data-wrapper-0.4.5/example.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      809 2023-06-21 20:57:10.000000 amplitude-data-wrapper-0.4.5/pyproject.toml
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:57:31.749616 amplitude-data-wrapper-0.4.5/requirements/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3391 2023-06-21 19:22:04.000000 amplitude-data-wrapper-0.4.5/requirements/dev.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      438 2023-06-21 19:21:45.000000 amplitude-data-wrapper-0.4.5/requirements/main.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-06-21 20:57:31.774971 amplitude-data-wrapper-0.4.5/setup.cfg
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:57:31.723863 amplitude-data-wrapper-0.4.5/src/
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:57:31.760095 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:08:45.000000 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper/analytics_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-21 20:57:31.772654 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5901 2023-06-21 20:57:31.000000 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      449 2023-06-21 20:57:31.000000 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-21 20:57:31.000000 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       75 2023-06-21 20:57:31.000000 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper.egg-info/requires.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-06-21 20:57:31.000000 amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper.egg-info/top_level.txt
```

### Comparing `amplitude-data-wrapper-0.4.4/LICENSE` & `amplitude-data-wrapper-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.4/Makefile` & `amplitude-data-wrapper-0.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.4/PKG-INFO` & `amplitude-data-wrapper-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplitude-data-wrapper
-Version: 0.4.4
+Version: 0.4.5
 Summary: python wrapper for using the amplitude analytics and taxonomy APIs
 Author-email: Tobias McVey <tobias.mcvey@nav.no>
 License: MIT License
         
         Copyright (c) 2022 NAV IT
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `amplitude-data-wrapper-0.4.4/README.md` & `amplitude-data-wrapper-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.4/example.py` & `amplitude-data-wrapper-0.4.5/example.py`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.4/pyproject.toml` & `amplitude-data-wrapper-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amplitude-data-wrapper"
-version = "0.4.4"
+version = "0.4.5"
 description = "python wrapper for using the amplitude analytics and taxonomy APIs"
 authors = [
     {name = "Tobias McVey", email = "tobias.mcvey@nav.no"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["amplitude"]
```

### Comparing `amplitude-data-wrapper-0.4.4/requirements/dev.txt` & `amplitude-data-wrapper-0.4.5/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper/analytics_api.py` & `amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper/analytics_api.py`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.4/src/amplitude_data_wrapper.egg-info/PKG-INFO` & `amplitude-data-wrapper-0.4.5/src/amplitude_data_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplitude-data-wrapper
-Version: 0.4.4
+Version: 0.4.5
 Summary: python wrapper for using the amplitude analytics and taxonomy APIs
 Author-email: Tobias McVey <tobias.mcvey@nav.no>
 License: MIT License
         
         Copyright (c) 2022 NAV IT
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

