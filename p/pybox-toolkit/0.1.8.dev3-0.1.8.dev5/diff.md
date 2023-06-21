# Comparing `tmp/pybox-toolkit-0.1.8.dev3.tar.gz` & `tmp/pybox-toolkit-0.1.8.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.8.dev3.tar", last modified: Mon Jun 19 09:47:56 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.8.dev5.tar", last modified: Mon Jun 19 10:05:14 2023, max compression
```

## Comparing `pybox-toolkit-0.1.8.dev3.tar` & `pybox-toolkit-0.1.8.dev5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:47:56.127439 pybox-toolkit-0.1.8.dev3/
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-19 09:47:56.127439 pybox-toolkit-0.1.8.dev3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-11 12:19:14.000000 pybox-toolkit-0.1.8.dev3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-11 12:19:14.000000 pybox-toolkit-0.1.8.dev3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 09:47:56.127439 pybox-toolkit-0.1.8.dev3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:47:56.119439 pybox-toolkit-0.1.8.dev3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:47:56.123439 pybox-toolkit-0.1.8.dev3/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-19 09:47:56.000000 pybox-toolkit-0.1.8.dev3/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-19 09:47:56.000000 pybox-toolkit-0.1.8.dev3/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:47:56.000000 pybox-toolkit-0.1.8.dev3/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-19 09:47:56.000000 pybox-toolkit-0.1.8.dev3/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-19 09:47:56.000000 pybox-toolkit-0.1.8.dev3/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:47:56.123439 pybox-toolkit-0.1.8.dev3/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15085 2023-06-19 09:46:10.000000 pybox-toolkit-0.1.8.dev3/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:47:56.123439 pybox-toolkit-0.1.8.dev3/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-11 12:19:14.000000 pybox-toolkit-0.1.8.dev3/src/toolkit/graphing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:47:56.123439 pybox-toolkit-0.1.8.dev3/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5222 2023-06-19 08:28:37.000000 pybox-toolkit-0.1.8.dev3/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:47:56.127439 pybox-toolkit-0.1.8.dev3/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-12 14:15:14.000000 pybox-toolkit-0.1.8.dev3/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-11 12:19:14.000000 pybox-toolkit-0.1.8.dev3/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-12 14:15:14.000000 pybox-toolkit-0.1.8.dev3/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.877593 pybox-toolkit-0.1.8.dev5/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-19 10:05:14.877593 pybox-toolkit-0.1.8.dev5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 10:05:14.877593 pybox-toolkit-0.1.8.dev5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.869593 pybox-toolkit-0.1.8.dev5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.873593 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.873593 pybox-toolkit-0.1.8.dev5/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15168 2023-06-19 10:04:42.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.873593 pybox-toolkit-0.1.8.dev5/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/graphing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.873593 pybox-toolkit-0.1.8.dev5/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.877593 pybox-toolkit-0.1.8.dev5/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.8.dev3/pyproject.toml` & `pybox-toolkit-0.1.8.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev3/src/toolkit/__init__.py` & `pybox-toolkit-0.1.8.dev5/src/toolkit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,16 @@
 
         Args:
             output_list (list[dict[str, BaseUnit]]]): list of outputs
 
         Returns:
             list[dict[str, BaseUnit]]: lists of outputs in their physical range
         """
-        results = list(filter(self.filter_variable_dictionary, output_list))
+        floatified = map(lambda dic: map_dictionary_value(float, dic), output_list)
+        results = list(filter(self.filter_variable_dictionary, floatified))
 
         if len(results) == 0:
             raise RuntimeException(
                 f"No outputs were produced for '{self.name}'. The arguments may have been insufficient to solve the equation"  # pylint: disable=line-too-long
             )
 
         return results
```

### Comparing `pybox-toolkit-0.1.8.dev3/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.8.dev5/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev3/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.8.dev5/src/toolkit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev3/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.8.dev5/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev3/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.8.dev5/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev3/src/toolkit/utils.py` & `pybox-toolkit-0.1.8.dev5/src/toolkit/utils.py`

 * *Files identical despite different names*

