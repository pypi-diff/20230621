# Comparing `tmp/spectroscopy-toolbox-0.0.1.tar.gz` & `tmp/spectroscopy-toolbox-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectroscopy-toolbox-0.0.1.tar", last modified: Fri Jun 16 10:55:35 2023, max compression
+gzip compressed data, was "spectroscopy-toolbox-0.0.2a0.tar", last modified: Wed Jun 21 10:02:50 2023, max compression
```

## Comparing `spectroscopy-toolbox-0.0.1.tar` & `spectroscopy-toolbox-0.0.2a0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:55:35.995107 spectroscopy-toolbox-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 10:55:27.000000 spectroscopy-toolbox-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-16 10:55:35.995107 spectroscopy-toolbox-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-16 10:55:27.000000 spectroscopy-toolbox-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 10:55:27.000000 spectroscopy-toolbox-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-16 10:55:35.995107 spectroscopy-toolbox-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-16 10:55:27.000000 spectroscopy-toolbox-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:55:35.995107 spectroscopy-toolbox-0.0.1/spectroscopy_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-16 10:55:35.000000 spectroscopy-toolbox-0.0.1/spectroscopy_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-16 10:55:35.000000 spectroscopy-toolbox-0.0.1/spectroscopy_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 10:55:35.000000 spectroscopy-toolbox-0.0.1/spectroscopy_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 10:55:35.000000 spectroscopy-toolbox-0.0.1/spectroscopy_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 10:55:35.000000 spectroscopy-toolbox-0.0.1/spectroscopy_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 10:55:35.000000 spectroscopy-toolbox-0.0.1/spectroscopy_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:55:35.995107 spectroscopy-toolbox-0.0.1/spectroscopytools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 10:55:27.000000 spectroscopy-toolbox-0.0.1/spectroscopytools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-06-16 10:55:27.000000 spectroscopy-toolbox-0.0.1/spectroscopytools/uvvis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:02:50.818643 spectroscopy-toolbox-0.0.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 10:02:40.000000 spectroscopy-toolbox-0.0.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 10:02:50.818643 spectroscopy-toolbox-0.0.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-21 10:02:40.000000 spectroscopy-toolbox-0.0.2a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 10:02:40.000000 spectroscopy-toolbox-0.0.2a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-21 10:02:50.822643 spectroscopy-toolbox-0.0.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-21 10:02:40.000000 spectroscopy-toolbox-0.0.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:02:50.818643 spectroscopy-toolbox-0.0.2a0/spectroscopy_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 10:02:50.000000 spectroscopy-toolbox-0.0.2a0/spectroscopy_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-21 10:02:50.000000 spectroscopy-toolbox-0.0.2a0/spectroscopy_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:02:50.000000 spectroscopy-toolbox-0.0.2a0/spectroscopy_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:02:50.000000 spectroscopy-toolbox-0.0.2a0/spectroscopy_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 10:02:50.000000 spectroscopy-toolbox-0.0.2a0/spectroscopy_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 10:02:50.000000 spectroscopy-toolbox-0.0.2a0/spectroscopy_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:02:50.818643 spectroscopy-toolbox-0.0.2a0/spectroscopytools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:02:40.000000 spectroscopy-toolbox-0.0.2a0/spectroscopytools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-21 10:02:40.000000 spectroscopy-toolbox-0.0.2a0/spectroscopytools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31090 2023-06-21 10:02:40.000000 spectroscopy-toolbox-0.0.2a0/spectroscopytools/uvvis.py
```

### Comparing `spectroscopy-toolbox-0.0.1/LICENSE` & `spectroscopy-toolbox-0.0.2a0/LICENSE`

 * *Files identical despite different names*

