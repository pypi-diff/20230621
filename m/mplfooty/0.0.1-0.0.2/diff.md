# Comparing `tmp/mplfooty-0.0.1.tar.gz` & `tmp/mplfooty-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mplfooty-0.0.1.tar", last modified: Tue Jun 20 07:10:11 2023, max compression
+gzip compressed data, was "mplfooty-0.0.2.tar", last modified: Wed Jun 21 07:38:40 2023, max compression
```

## Comparing `mplfooty-0.0.1.tar` & `mplfooty-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-20 07:10:11.587948 mplfooty-0.0.1/
--rw-r--r--   0 ciaran     (501) staff       (20)     1069 2023-06-20 07:00:35.000000 mplfooty-0.0.1/LICENSE
--rw-r--r--   0 ciaran     (501) staff       (20)     1740 2023-06-20 07:10:11.587747 mplfooty-0.0.1/PKG-INFO
--rw-r--r--   0 ciaran     (501) staff       (20)      170 2023-06-20 07:00:35.000000 mplfooty-0.0.1/README.md
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-20 07:10:11.586523 mplfooty-0.0.1/mplfooty/
--rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-06-20 06:57:42.000000 mplfooty-0.0.1/mplfooty/__init__.py
--rw-r--r--   0 ciaran     (501) staff       (20)     4111 2023-06-20 06:57:42.000000 mplfooty-0.0.1/mplfooty/dimensions.py
--rw-r--r--   0 ciaran     (501) staff       (20)     2762 2023-06-20 06:57:42.000000 mplfooty-0.0.1/mplfooty/pitch.py
--rw-r--r--   0 ciaran     (501) staff       (20)    35636 2023-06-20 06:57:42.000000 mplfooty-0.0.1/mplfooty/pitch_base.py
--rw-r--r--   0 ciaran     (501) staff       (20)    43682 2023-06-20 06:57:42.000000 mplfooty-0.0.1/mplfooty/pitch_plot.py
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-20 07:10:11.587469 mplfooty-0.0.1/mplfooty.egg-info/
--rw-r--r--   0 ciaran     (501) staff       (20)     1740 2023-06-20 07:10:11.000000 mplfooty-0.0.1/mplfooty.egg-info/PKG-INFO
--rw-r--r--   0 ciaran     (501) staff       (20)      299 2023-06-20 07:10:11.000000 mplfooty-0.0.1/mplfooty.egg-info/SOURCES.txt
--rw-r--r--   0 ciaran     (501) staff       (20)        1 2023-06-20 07:10:11.000000 mplfooty-0.0.1/mplfooty.egg-info/dependency_links.txt
--rw-r--r--   0 ciaran     (501) staff       (20)      206 2023-06-20 07:10:11.000000 mplfooty-0.0.1/mplfooty.egg-info/requires.txt
--rw-r--r--   0 ciaran     (501) staff       (20)        9 2023-06-20 07:10:11.000000 mplfooty-0.0.1/mplfooty.egg-info/top_level.txt
--rw-r--r--   0 ciaran     (501) staff       (20)      774 2023-06-20 07:04:28.000000 mplfooty-0.0.1/pyproject.toml
--rw-r--r--   0 ciaran     (501) staff       (20)       38 2023-06-20 07:10:11.588006 mplfooty-0.0.1/setup.cfg
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-21 07:38:40.405919 mplfooty-0.0.2/
+-rw-r--r--   0 ciaran     (501) staff       (20)     1069 2023-06-20 07:00:35.000000 mplfooty-0.0.2/LICENSE
+-rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-06-21 07:38:40.405771 mplfooty-0.0.2/PKG-INFO
+-rw-r--r--   0 ciaran     (501) staff       (20)     3228 2023-06-21 07:32:42.000000 mplfooty-0.0.2/README.md
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-21 07:38:40.404553 mplfooty-0.0.2/mplfooty/
+-rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/__init__.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     4111 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/dimensions.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     2762 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/pitch.py
+-rw-r--r--   0 ciaran     (501) staff       (20)    35636 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/pitch_base.py
+-rw-r--r--   0 ciaran     (501) staff       (20)    43682 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/pitch_plot.py
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-21 07:38:40.405561 mplfooty-0.0.2/mplfooty.egg-info/
+-rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/PKG-INFO
+-rw-r--r--   0 ciaran     (501) staff       (20)      299 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/SOURCES.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)        1 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/dependency_links.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)      206 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/requires.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)        9 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/top_level.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)      774 2023-06-21 07:38:05.000000 mplfooty-0.0.2/pyproject.toml
+-rw-r--r--   0 ciaran     (501) staff       (20)       38 2023-06-21 07:38:40.405961 mplfooty-0.0.2/setup.cfg
```

### Comparing `mplfooty-0.0.1/LICENSE` & `mplfooty-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.1/mplfooty/dimensions.py` & `mplfooty-0.0.2/mplfooty/dimensions.py`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.1/mplfooty/pitch.py` & `mplfooty-0.0.2/mplfooty/pitch.py`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.1/mplfooty/pitch_base.py` & `mplfooty-0.0.2/mplfooty/pitch_base.py`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.1/mplfooty/pitch_plot.py` & `mplfooty-0.0.2/mplfooty/pitch_plot.py`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.1/pyproject.toml` & `mplfooty-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mplfooty"
-version = "0.0.1"
+version = "0.0.2"
 description = "AFL pitch plotting using matplotlib"
 readme = "README.md"
 authors = [{name = "Ciaran Grant", email = "ciaran.grant@hotmail.co.uk"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 dependencies = [
     "pandas == 1.5.3",
```

