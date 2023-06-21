# Comparing `tmp/boneflet-0.1.0.dev3.tar.gz` & `tmp/boneflet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneflet-0.1.0.dev3.tar", last modified: Tue May 23 13:51:11 2023, max compression
+gzip compressed data, was "boneflet-0.1.1.tar", last modified: Wed Jun 21 14:45:04 2023, max compression
```

## Comparing `boneflet-0.1.0.dev3.tar` & `boneflet-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       31 2023-04-10 12:59:29.626977 boneflet-0.1.0.dev3/README.md
--rw-r--r--   0        0        0       26 2023-05-22 15:08:45.043751 boneflet-0.1.0.dev3/boneflet/__init__.py
--rw-r--r--   0        0        0     2616 2023-01-28 16:32:10.074370 boneflet-0.1.0.dev3/boneflet/bonetools.py
--rw-r--r--   0        0        0     2371 2023-01-20 11:10:31.713541 boneflet-0.1.0.dev3/boneflet/button.py
--rw-r--r--   0        0        0     2612 2023-04-06 16:34:56.554777 boneflet-0.1.0.dev3/boneflet/demo.py
--rw-r--r--   0        0        0      141 2023-01-28 14:56:25.378961 boneflet-0.1.0.dev3/boneflet/plugins/__init__.py
--rw-r--r--   0        0        0     3343 2023-04-13 08:23:33.494812 boneflet-0.1.0.dev3/boneflet/plugins/demo.py
--rw-r--r--   0        0        0      141 2023-04-06 16:30:26.604380 boneflet-0.1.0.dev3/boneflet/plugins/ui_demo.py
--rw-r--r--   0        0        0     6243 2023-04-07 09:33:24.572849 boneflet-0.1.0.dev3/boneflet/tab.py
--rw-r--r--   0        0        0      417 2023-05-23 13:51:11.426689 boneflet-0.1.0.dev3/pyproject.toml
--rw-r--r--   0        0        0      239 1970-01-01 00:00:00.000000 boneflet-0.1.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0       31 2023-04-10 12:59:29.626977 boneflet-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-21 14:40:32.258133 boneflet-0.1.1/boneflet/__init__.py
+-rw-r--r--   0        0        0     2616 2023-01-28 16:32:10.074370 boneflet-0.1.1/boneflet/bonetools.py
+-rw-r--r--   0        0        0     2371 2023-01-20 11:10:31.713541 boneflet-0.1.1/boneflet/button.py
+-rw-r--r--   0        0        0     2612 2023-04-06 16:34:56.554777 boneflet-0.1.1/boneflet/demo.py
+-rw-r--r--   0        0        0      141 2023-01-28 14:56:25.378961 boneflet-0.1.1/boneflet/plugins/__init__.py
+-rw-r--r--   0        0        0     3343 2023-04-13 08:23:33.494812 boneflet-0.1.1/boneflet/plugins/demo.py
+-rw-r--r--   0        0        0      141 2023-04-06 16:30:26.604380 boneflet-0.1.1/boneflet/plugins/ui_demo.py
+-rw-r--r--   0        0        0     6243 2023-04-07 09:33:24.572849 boneflet-0.1.1/boneflet/tab.py
+-rw-r--r--   0        0        0      413 2023-06-21 14:45:04.723452 boneflet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      234 1970-01-01 00:00:00.000000 boneflet-0.1.1/PKG-INFO
```

### Comparing `boneflet-0.1.0.dev3/boneflet/bonetools.py` & `boneflet-0.1.1/boneflet/bonetools.py`

 * *Files identical despite different names*

### Comparing `boneflet-0.1.0.dev3/boneflet/button.py` & `boneflet-0.1.1/boneflet/button.py`

 * *Files identical despite different names*

### Comparing `boneflet-0.1.0.dev3/boneflet/demo.py` & `boneflet-0.1.1/boneflet/demo.py`

 * *Files identical despite different names*

### Comparing `boneflet-0.1.0.dev3/boneflet/plugins/demo.py` & `boneflet-0.1.1/boneflet/plugins/demo.py`

 * *Files identical despite different names*

### Comparing `boneflet-0.1.0.dev3/boneflet/tab.py` & `boneflet-0.1.1/boneflet/tab.py`

 * *Files identical despite different names*

