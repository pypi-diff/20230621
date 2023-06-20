# Comparing `tmp/temper_core-0.0.4.tar.gz` & `tmp/temper_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_core-0.0.4.tar", max compression
+gzip compressed data, was "temper_core-0.0.5.tar", max compression
```

## Comparing `temper_core-0.0.4.tar` & `temper_core-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      428 2023-06-09 16:40:49.254815 temper_core-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    25341 2023-06-09 16:40:49.256811 temper_core-0.0.4/temper_core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 16:40:49.255812 temper_core-0.0.4/temper_core/py.typed
--rw-r--r--   0        0        0     1544 2023-06-09 16:40:49.257810 temper_core-0.0.4/temper_core/regex.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 temper_core-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      428 2023-06-20 22:03:46.990783 temper_core-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    25341 2023-06-20 22:03:46.993783 temper_core-0.0.5/temper_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:03:46.991784 temper_core-0.0.5/temper_core/py.typed
+-rw-r--r--   0        0        0     1544 2023-06-20 22:03:46.995784 temper_core-0.0.5/temper_core/regex.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 temper_core-0.0.5/PKG-INFO
```

### Comparing `temper_core-0.0.4/temper_core/__init__.py` & `temper_core-0.0.5/temper_core/__init__.py`

 * *Files identical despite different names*

### Comparing `temper_core-0.0.4/temper_core/regex.py` & `temper_core-0.0.5/temper_core/regex.py`

 * *Files identical despite different names*

