# Comparing `tmp/pynterface-0.2.0.tar.gz` & `tmp/pynterface-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynterface-0.2.0.tar", last modified: Sat May 20 02:21:10 2023, max compression
+gzip compressed data, was "pynterface-0.2.1.tar", last modified: Wed Jun 21 16:29:05 2023, max compression
```

## Comparing `pynterface-0.2.0.tar` & `pynterface-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-20 02:21:10.410116 pynterface-0.2.0/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.2.0/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.2.0/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-20 02:21:10.409834 pynterface-0.2.0/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.2.0/README.md
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-20 02:21:10.408396 pynterface-0.2.0/pynterface/
--rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-20 02:20:02.000000 pynterface-0.2.0/pynterface/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3398 2023-05-20 02:19:35.000000 pynterface-0.2.0/pynterface/input.py
--rw-r--r--   0 vivaan     (501) staff       (20)     6438 2023-05-17 14:21:57.000000 pynterface-0.2.0/pynterface/loading.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.2.0/pynterface/menu.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.2.0/pynterface/printing.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.2.0/pynterface/style.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-20 02:21:10.409493 pynterface-0.2.0/pynterface.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-20 02:21:10.000000 pynterface-0.2.0/pynterface.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-20 02:21:10.000000 pynterface-0.2.0/pynterface.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-20 02:21:10.000000 pynterface-0.2.0/pynterface.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-20 02:21:10.000000 pynterface-0.2.0/pynterface.egg-info/top_level.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-20 02:21:10.410198 pynterface-0.2.0/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.2.0/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-06-21 16:29:05.627263 pynterface-0.2.1/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.2.1/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.2.1/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-06-21 16:29:05.627021 pynterface-0.2.1/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.2.1/README.md
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-06-21 16:29:05.625453 pynterface-0.2.1/pynterface/
+-rw-r--r--   0 vivaan     (501) staff       (20)      239 2023-06-21 16:28:17.000000 pynterface-0.2.1/pynterface/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     3410 2023-06-21 16:26:51.000000 pynterface-0.2.1/pynterface/input.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     6438 2023-05-17 14:21:57.000000 pynterface-0.2.1/pynterface/loading.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.2.1/pynterface/menu.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.2.1/pynterface/printing.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.2.1/pynterface/style.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-06-21 16:29:05.626601 pynterface-0.2.1/pynterface.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-06-21 16:29:05.000000 pynterface-0.2.1/pynterface.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-06-21 16:29:05.000000 pynterface-0.2.1/pynterface.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-06-21 16:29:05.000000 pynterface-0.2.1/pynterface.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-06-21 16:29:05.000000 pynterface-0.2.1/pynterface.egg-info/top_level.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-06-21 16:29:05.627348 pynterface-0.2.1/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.2.1/setup.py
```

### Comparing `pynterface-0.2.0/LICENSE` & `pynterface-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.0/PKG-INFO` & `pynterface-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.2.0
+Version: 0.2.1
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.2.0/README.md` & `pynterface-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.0/pynterface/input.py` & `pynterface-0.2.1/pynterface/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             if isinstance(user_input, float):       # get first input
                 user_input = int(input(prompt))
             elif flag_type_error:
                 user_input = int(input(type_error))     
                 flag_type_error = False
             else:
                 user_input = int(input(bounds_error))
-        except:
+        except ValueError:
             user_input = lower - 1      # reset to a set out of bounds value
             flag_type_error = True
 
     return user_input
 
 def two_dim_array(rows: int, cols: int = None, delimiter: str = " ", item_type: int = str) -> list[list[Any]]:
 
@@ -84,8 +84,8 @@
     no = ['no', 'n', '0']
 
     choice = input(prompt).lower()
     
     while choice not in yes+no:
         choice = input(error_prompt).lower()
 
-    return choice in yes
+    return choice in yes
```

### Comparing `pynterface-0.2.0/pynterface/loading.py` & `pynterface-0.2.1/pynterface/loading.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.0/pynterface/menu.py` & `pynterface-0.2.1/pynterface/menu.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.0/pynterface/printing.py` & `pynterface-0.2.1/pynterface/printing.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.0/pynterface/style.py` & `pynterface-0.2.1/pynterface/style.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.0/pynterface.egg-info/PKG-INFO` & `pynterface-0.2.1/pynterface.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.2.0
+Version: 0.2.1
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.2.0/setup.py` & `pynterface-0.2.1/setup.py`

 * *Files identical despite different names*

