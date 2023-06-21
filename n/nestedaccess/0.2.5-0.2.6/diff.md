# Comparing `tmp/nestedaccess-0.2.5.tar.gz` & `tmp/nestedaccess-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.2.5.tar", last modified: Fri Jun 16 06:37:03 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.2.6.tar", last modified: Wed Jun 21 03:52:22 2023, max compression
```

## Comparing `nestedaccess-0.2.5.tar` & `nestedaccess-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:37:03.634127 nestedaccess-0.2.5/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.5/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.5/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:37:03.633855 nestedaccess-0.2.5/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.2.5/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:37:03.631731 nestedaccess-0.2.5/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 06:35:15.000000 nestedaccess-0.2.5/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 06:35:17.000000 nestedaccess-0.2.5/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 06:37:03.633406 nestedaccess-0.2.5/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       73 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/entry_points.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 06:37:03.000000 nestedaccess-0.2.5/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 06:37:03.634213 nestedaccess-0.2.5/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3684 2023-06-16 06:37:01.000000 nestedaccess-0.2.5/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 03:52:22.400953 nestedaccess-0.2.6/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.2.6/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.2.6/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 03:52:22.400601 nestedaccess-0.2.6/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:41.000000 nestedaccess-0.2.6/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 03:52:22.396320 nestedaccess-0.2.6/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       41 2023-06-21 03:42:02.000000 nestedaccess-0.2.6/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:00.000000 nestedaccess-0.2.6/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 03:52:22.399962 nestedaccess-0.2.6/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2824 2023-06-21 03:52:22.000000 nestedaccess-0.2.6/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-21 03:52:22.000000 nestedaccess-0.2.6/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-21 03:52:22.000000 nestedaccess-0.2.6/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       73 2023-06-21 03:52:22.000000 nestedaccess-0.2.6/nestedaccess.egg-info/entry_points.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-21 03:52:22.000000 nestedaccess-0.2.6/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-21 03:52:22.401058 nestedaccess-0.2.6/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3684 2023-06-21 03:44:49.000000 nestedaccess-0.2.6/setup.py
```

### Comparing `nestedaccess-0.2.5/LICENSE` & `nestedaccess-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.2.5/PKG-INFO` & `nestedaccess-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.2.5
+Version: 0.2.6
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
@@ -27,21 +27,21 @@
                 }
             },
             'empty_list': [],
             'empty_dict': {}
         }
         
         # normal test
-        print(nestedaccess(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
+        print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
         
         # default test
-        print(nestedaccess(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
+        print(nestedaccess.get(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
         
         # error condition test
-        print(nestedaccess(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+        print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
         ```
         
         # Installing Nestedaccess and Supported Versions
         
         ## Nestedaccess is available on PyPI:
         
         ```python
```

### Comparing `nestedaccess-0.2.5/README.md` & `nestedaccess-0.2.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,21 @@
         }
     },
     'empty_list': [],
     'empty_dict': {}
 }
 
 # normal test
-print(nestedaccess(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
+print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
 
 # default test
-print(nestedaccess(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
+print(nestedaccess.get(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
 
 # error condition test
-print(nestedaccess(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
 ```
 
 # Installing Nestedaccess and Supported Versions
 
 ## Nestedaccess is available on PyPI:
 
 ```python
```

### Comparing `nestedaccess-0.2.5/nestedaccess/nestedaccess.py` & `nestedaccess-0.2.6/nestedaccess/nestedaccess.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-def nestedaccess(data, keys, default=None):
+def get(data, keys, default=None):
     """
     get nested data
 
     Args:
         data (dict or list): Nested data objects, which can be dictionaries or lists
         keys (list): list of keys or indices to fetch nested data
         default (any, optional): The default value, returned when the acquisition fails, the default is None
 
     Returns:
         any: Nested data value, if the acquisition fails, return the default value
 
     Example:
         data = {'foo': {'bar': [1, 2, 3]}}
-        value = get_nested_data(data, ['foo', 'bar', 1])
+        value = get(data, ['foo', 'bar', 1])
         print(value)  # Output: 2
     """
     try:
         for key in keys:
             if isinstance(data, dict):
                 data = data.get(key, default)
                 if data is default:
```

### Comparing `nestedaccess-0.2.5/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.2.6/nestedaccess.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.2.5
+Version: 0.2.6
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
@@ -27,21 +27,21 @@
                 }
             },
             'empty_list': [],
             'empty_dict': {}
         }
         
         # normal test
-        print(nestedaccess(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
+        print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
         
         # default test
-        print(nestedaccess(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
+        print(nestedaccess.get(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
         
         # error condition test
-        print(nestedaccess(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+        print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
         ```
         
         # Installing Nestedaccess and Supported Versions
         
         ## Nestedaccess is available on PyPI:
         
         ```python
```

### Comparing `nestedaccess-0.2.5/setup.py` & `nestedaccess-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.2.5"
+VERSION = "0.2.6"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
```

