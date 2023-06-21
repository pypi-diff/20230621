# Comparing `tmp/scriptpak-0.2.tar.gz` & `tmp/scriptpak-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptpak-0.2.tar", last modified: Wed Jun 21 12:49:32 2023, max compression
+gzip compressed data, was "scriptpak-0.3.tar", last modified: Wed Jun 21 12:51:37 2023, max compression
```

## Comparing `scriptpak-0.2.tar` & `scriptpak-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-21 12:49:32.050256 scriptpak-0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)      749 2023-06-21 12:49:32.050256 scriptpak-0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      528 2023-06-20 14:03:10.000000 scriptpak-0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-21 12:49:32.026256 scriptpak-0.2/scriptpak/
--rw-r--r--   0 runner    (1000) runner    (1000)     2165 2023-06-14 20:08:10.000000 scriptpak-0.2/scriptpak/__main__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-21 12:49:32.050256 scriptpak-0.2/scriptpak.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      749 2023-06-21 12:49:31.000000 scriptpak-0.2/scriptpak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      209 2023-06-21 12:49:31.000000 scriptpak-0.2/scriptpak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-21 12:49:31.000000 scriptpak-0.2/scriptpak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2023-06-21 12:49:31.000000 scriptpak-0.2/scriptpak.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-21 12:49:31.000000 scriptpak-0.2/scriptpak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-21 12:49:32.050256 scriptpak-0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      536 2023-06-21 12:48:48.000000 scriptpak-0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-21 12:51:37.758029 scriptpak-0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)      710 2023-06-21 12:51:37.758029 scriptpak-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      528 2023-06-20 14:03:10.000000 scriptpak-0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-21 12:51:37.754029 scriptpak-0.3/scriptpak/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2165 2023-06-14 20:08:10.000000 scriptpak-0.3/scriptpak/__main__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-21 12:51:37.758029 scriptpak-0.3/scriptpak.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      710 2023-06-21 12:51:37.000000 scriptpak-0.3/scriptpak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      209 2023-06-21 12:51:37.000000 scriptpak-0.3/scriptpak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-21 12:51:37.000000 scriptpak-0.3/scriptpak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2023-06-21 12:51:37.000000 scriptpak-0.3/scriptpak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-21 12:51:37.000000 scriptpak-0.3/scriptpak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-21 12:51:37.758029 scriptpak-0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      563 2023-06-21 12:51:15.000000 scriptpak-0.3/setup.py
```

### Comparing `scriptpak-0.2/pyproject.toml` & `scriptpak-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scriptpak-0.2/scriptpak/__main__.py` & `scriptpak-0.3/scriptpak/__main__.py`

 * *Files identical despite different names*

### Comparing `scriptpak-0.2/setup.py` & `scriptpak-0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 import subprocess
 
 setuptools.setup(
 	name="scriptpak",
-	version="0.2",
+	version="0.3",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="The scriptpak programming language",
 	packages=["scriptpak"],
 	classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 	install_requires=["flask"],
-	long_description=subprocess.Popen(["python", "-m", "scriptpak"], stdout=subprocess.PIPE).communicate()[0].decode(),
+	long_description="\n".join(subprocess.Popen(["python", "-m", "scriptpak"], stdout=subprocess.PIPE).communicate()[0].decode().split("\n")[2:]),
 	long_description_content_type="text/plain"
 )
```

