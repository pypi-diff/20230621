# Comparing `tmp/cemconvert-0.5.5.tar.gz` & `tmp/cemconvert-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cemconvert-0.5.5.tar", last modified: Wed Jun 21 13:33:14 2023, max compression
+gzip compressed data, was "dist/cemconvert-0.5.6.tar", last modified: Wed Jun 21 14:13:28 2023, max compression
```

## Comparing `cemconvert-0.5.5.tar` & `cemconvert-0.5.6.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      671 2023-06-21 13:33:00.000000 cemconvert-0.5.5/setup.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 13:33:14.000000 cemconvert-0.5.5/PKG-INFO
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/bin/
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.5/bin/get_camd_cems
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.5/bin/cemconvert
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6349 2023-05-12 16:11:03.000000 cemconvert-0.5.5/bin/get_camd_cems_bulk
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/cemconvert/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/tz.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/temporal.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10736 2023-06-21 13:31:52.000000 cemconvert-0.5.5/cemconvert/ff10.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/qa.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/__init__.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.5/cemconvert/cemcorrect.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.5/cemconvert/proc.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6781 2023-05-19 20:23:16.000000 cemconvert-0.5.5/cemconvert/cem.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-06-20 16:36:27.000000 cemconvert-0.5.5/cemconvert/run_parse.py
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/examples/
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)      307 2023-06-20 16:30:32.000000 cemconvert-0.5.5/examples/get_camd_cems.csh
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     1188 2023-06-16 19:57:48.000000 cemconvert-0.5.5/examples/cemconvert_2021.csh
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-06-21 13:33:14.000000 cemconvert-0.5.5/setup.cfg
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2499 2023-06-20 16:44:51.000000 cemconvert-0.5.5/README.md
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 13:33:14.000000 cemconvert-0.5.5/cemconvert.egg-info/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      484 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/SOURCES.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/PKG-INFO
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/dependency_links.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       11 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/top_level.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       28 2023-06-21 13:33:13.000000 cemconvert-0.5.5/cemconvert.egg-info/requires.txt
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      628 2023-06-21 14:13:02.000000 cemconvert-0.5.6/setup.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 14:13:28.000000 cemconvert-0.5.6/PKG-INFO
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/bin/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.6/bin/get_camd_cems
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.6/bin/cemconvert
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6349 2023-05-12 16:11:03.000000 cemconvert-0.5.6/bin/get_camd_cems_bulk
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-06-21 14:13:28.000000 cemconvert-0.5.6/setup.cfg
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2499 2023-06-20 16:44:51.000000 cemconvert-0.5.6/README.md
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/tz.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/temporal.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10736 2023-06-21 13:31:52.000000 cemconvert-0.5.6/src/cemconvert/ff10.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/qa.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/__init__.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.6/src/cemconvert/cemcorrect.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.6/src/cemconvert/proc.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert/examples/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)      307 2023-06-20 16:30:32.000000 cemconvert-0.5.6/src/cemconvert/examples/get_camd_cems.csh
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     1188 2023-06-16 19:57:48.000000 cemconvert-0.5.6/src/cemconvert/examples/cemconvert_2021.csh
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6781 2023-05-19 20:23:16.000000 cemconvert-0.5.6/src/cemconvert/cem.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert/data/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)    95049 2023-02-08 15:30:00.000000 cemconvert-0.5.6/src/cemconvert/data/county_fips_tz.csv
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-06-20 16:36:27.000000 cemconvert-0.5.6/src/cemconvert/run_parse.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      609 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/PKG-INFO
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       11 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/top_level.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       28 2023-06-21 14:13:28.000000 cemconvert-0.5.6/src/cemconvert.egg-info/requires.txt
```

### Comparing `cemconvert-0.5.5/setup.py` & `cemconvert-0.5.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages, Extension
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name="cemconvert",
-    version="0.5.5",
-    packages = find_packages(),
+    version="0.5.6",
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
     python_requires='>=3.5',
     scripts=['bin/cemconvert','bin/get_camd_cems','bin/get_camd_cems_bulk'],
     setup_requires=['numpy>=1.19.5','pandas>=1.1.0'],
     install_requires=['numpy>=1.19.5','pandas>=1.1.0'],
-    package_data={'cemconvert': ['examples/*.csh']},
-    data_files=[('examples', ['examples/cemconvert_2021.csh','examples/get_camd_cems.csh'])],
+    package_data={'cemconvert': ['examples/*.csh','data/*.csv']},
     author_email='beidler.james@epa.gov'
 )
```

### Comparing `cemconvert-0.5.5/bin/get_camd_cems` & `cemconvert-0.5.6/bin/get_camd_cems`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/bin/cemconvert` & `cemconvert-0.5.6/bin/cemconvert`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/bin/get_camd_cems_bulk` & `cemconvert-0.5.6/bin/get_camd_cems_bulk`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/cemconvert/tz.py` & `cemconvert-0.5.6/src/cemconvert/tz.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/cemconvert/temporal.py` & `cemconvert-0.5.6/src/cemconvert/temporal.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/cemconvert/ff10.py` & `cemconvert-0.5.6/src/cemconvert/ff10.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/cemconvert/qa.py` & `cemconvert-0.5.6/src/cemconvert/qa.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/cemconvert/cemcorrect.py` & `cemconvert-0.5.6/src/cemconvert/cemcorrect.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/cemconvert/proc.py` & `cemconvert-0.5.6/src/cemconvert/proc.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/cemconvert/cem.py` & `cemconvert-0.5.6/src/cemconvert/cem.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/cemconvert/run_parse.py` & `cemconvert-0.5.6/src/cemconvert/run_parse.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/examples/cemconvert_2021.csh` & `cemconvert-0.5.6/src/cemconvert/examples/cemconvert_2021.csh`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.5/README.md` & `cemconvert-0.5.6/README.md`

 * *Files identical despite different names*

