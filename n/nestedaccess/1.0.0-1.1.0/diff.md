# Comparing `tmp/nestedaccess-1.0.0.tar.gz` & `tmp/nestedaccess-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-1.0.0.tar", last modified: Wed Jun 21 07:12:12 2023, max compression
+gzip compressed data, was "dist/nestedaccess-1.1.0.tar", last modified: Wed Jun 21 08:14:04 2023, max compression
```

## Comparing `nestedaccess-1.0.0.tar` & `nestedaccess-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:12:12.947769 nestedaccess-1.0.0/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-1.0.0/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-1.0.0/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2836 2023-06-21 07:12:12.947514 nestedaccess-1.0.0/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 03:43:41.000000 nestedaccess-1.0.0/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:12:12.943628 nestedaccess-1.0.0/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       41 2023-06-21 07:06:24.000000 nestedaccess-1.0.0/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1487 2023-06-21 07:06:27.000000 nestedaccess-1.0.0/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 07:12:12.947085 nestedaccess-1.0.0/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2836 2023-06-21 07:12:12.000000 nestedaccess-1.0.0/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-21 07:12:12.000000 nestedaccess-1.0.0/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-21 07:12:12.000000 nestedaccess-1.0.0/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-21 07:12:12.000000 nestedaccess-1.0.0/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-21 07:12:12.947851 nestedaccess-1.0.0/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3494 2023-06-21 07:10:32.000000 nestedaccess-1.0.0/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 08:14:04.604257 nestedaccess-1.1.0/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-1.1.0/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-1.1.0/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     3478 2023-06-21 08:14:04.604012 nestedaccess-1.1.0/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     2081 2023-06-21 08:13:08.000000 nestedaccess-1.1.0/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 08:14:04.602132 nestedaccess-1.1.0/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       41 2023-06-21 07:06:24.000000 nestedaccess-1.1.0/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1562 2023-06-21 07:36:20.000000 nestedaccess-1.1.0/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-21 08:14:04.603591 nestedaccess-1.1.0/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     3478 2023-06-21 08:14:04.000000 nestedaccess-1.1.0/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-21 08:14:04.000000 nestedaccess-1.1.0/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-21 08:14:04.000000 nestedaccess-1.1.0/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-21 08:14:04.000000 nestedaccess-1.1.0/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-21 08:14:04.604338 nestedaccess-1.1.0/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3494 2023-06-21 08:13:24.000000 nestedaccess-1.1.0/setup.py
```

### Comparing `nestedaccess-1.0.0/LICENSE` & `nestedaccess-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-1.0.0/PKG-INFO` & `nestedaccess-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 1.0.0
+Version: 1.1.0
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
         
-        Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
+        Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries. If the field does not exist, you can customize the return to the default value, and you can also choose whether to output an error message.
         
         ```python
         
         import nestedaccess
         
         data = {
             'foo': {
@@ -26,22 +26,27 @@
                     }
                 }
             },
             'empty_list': [],
             'empty_dict': {}
         }
         
-        # normal test
+        # normal data test.
         print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
         
-        # default test
+        # Field does not exist, return default value data test.
         print(nestedaccess.get(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
         
-        # error condition test
-        print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+        # The field does not exist, no error message data test is returned.
+        print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None
+        
+        # The field does not exist and returns an error message test.
+        test_key = ['foo', 'baz', 'quux', 'corge', 'invalid']
+        print(nestedaccess.get(data, test_key, error_info=True))  # Output: None (dictionary key does not exist)
+        print(nestedaccess.get(data, test_key, error_info=True, default='Not found'))  # Output: 'Not found'
         ```
         
         # Installing Nestedaccess and Supported Versions
         
         ## Nestedaccess is available on PyPI:
         
         ```python
@@ -52,14 +57,15 @@
         
         # Supported Features & Best–Practices
         
         -   It is used to obtain nested data. In the case of a deep nested structure, the data is obtained through a list, which makes the code more elegant.
         -   Takes a nested data object (which can be a dictionary or a list), a list of keys or indices, and an optional default value.
         -   It will attempt to fetch nested data in the given key or index order, and fall back to the default value if fetching fails.
         -   If the field does not exist, output the non-existent field name and return the default value.
+        -   Customize the output error message (no error message is output by default).
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nestedaccess-1.0.0/README.md` & `nestedaccess-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Nestedaccess
 
-Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
+Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries. If the field does not exist, you can customize the return to the default value, and you can also choose whether to output an error message.
 
 ```python
 
 import nestedaccess
 
 data = {
     'foo': {
@@ -17,22 +17,27 @@
             }
         }
     },
     'empty_list': [],
     'empty_dict': {}
 }
 
-# normal test
+# normal data test.
 print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
 
-# default test
+# Field does not exist, return default value data test.
 print(nestedaccess.get(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
 
-# error condition test
-print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+# The field does not exist, no error message data test is returned.
+print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None
+
+# The field does not exist and returns an error message test.
+test_key = ['foo', 'baz', 'quux', 'corge', 'invalid']
+print(nestedaccess.get(data, test_key, error_info=True))  # Output: None (dictionary key does not exist)
+print(nestedaccess.get(data, test_key, error_info=True, default='Not found'))  # Output: 'Not found'
 ```
 
 # Installing Nestedaccess and Supported Versions
 
 ## Nestedaccess is available on PyPI:
 
 ```python
@@ -42,8 +47,9 @@
 Nestedaccess officially supports Python 3.7+.
 
 # Supported Features & Best–Practices
 
 -   It is used to obtain nested data. In the case of a deep nested structure, the data is obtained through a list, which makes the code more elegant.
 -   Takes a nested data object (which can be a dictionary or a list), a list of keys or indices, and an optional default value.
 -   It will attempt to fetch nested data in the given key or index order, and fall back to the default value if fetching fails.
--   If the field does not exist, output the non-existent field name and return the default value.
+-   If the field does not exist, output the non-existent field name and return the default value.
+-   Customize the output error message (no error message is output by default).
```

### Comparing `nestedaccess-1.0.0/nestedaccess/nestedaccess.py` & `nestedaccess-1.1.0/nestedaccess/nestedaccess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def get(data, keys, default=None):
+def get(data, keys, error_info=False, default=None):
     """
     get nested data
 
     Args:
         data (dict or list): Nested data objects, which can be dictionaries or lists
         keys (list): list of keys or indices to fetch nested data
         default (any, optional): The default value, returned when the acquisition fails, the default is None
@@ -30,10 +30,13 @@
                 else:
                     raise TypeError("list indices must be integers")
             else:
                 raise TypeError(
                     f"cannot fetch nested data because object of type {type(data).__name__} has no key or index"
                 )
     except (KeyError, IndexError, TypeError) as e:
-        print(f"an error occurred: {str(e)}")
+        if error_info:
+            print(f"an error occurred: {str(e)}")
+        else:
+            pass
         return default
-    return data
+    return data
```

### Comparing `nestedaccess-1.0.0/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-1.1.0/nestedaccess.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 1.0.0
+Version: 1.1.0
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
         
-        Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
+        Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries. If the field does not exist, you can customize the return to the default value, and you can also choose whether to output an error message.
         
         ```python
         
         import nestedaccess
         
         data = {
             'foo': {
@@ -26,22 +26,27 @@
                     }
                 }
             },
             'empty_list': [],
             'empty_dict': {}
         }
         
-        # normal test
+        # normal data test.
         print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
         
-        # default test
+        # Field does not exist, return default value data test.
         print(nestedaccess.get(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
         
-        # error condition test
-        print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+        # The field does not exist, no error message data test is returned.
+        print(nestedaccess.get(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None
+        
+        # The field does not exist and returns an error message test.
+        test_key = ['foo', 'baz', 'quux', 'corge', 'invalid']
+        print(nestedaccess.get(data, test_key, error_info=True))  # Output: None (dictionary key does not exist)
+        print(nestedaccess.get(data, test_key, error_info=True, default='Not found'))  # Output: 'Not found'
         ```
         
         # Installing Nestedaccess and Supported Versions
         
         ## Nestedaccess is available on PyPI:
         
         ```python
@@ -52,14 +57,15 @@
         
         # Supported Features & Best–Practices
         
         -   It is used to obtain nested data. In the case of a deep nested structure, the data is obtained through a list, which makes the code more elegant.
         -   Takes a nested data object (which can be a dictionary or a list), a list of keys or indices, and an optional default value.
         -   It will attempt to fetch nested data in the given key or index order, and fall back to the default value if fetching fails.
         -   If the field does not exist, output the non-existent field name and return the default value.
+        -   Customize the output error message (no error message is output by default).
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nestedaccess-1.0.0/setup.py` & `nestedaccess-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.0.0"
+VERSION = "1.1.0"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
```

