# Comparing `tmp/global_hotkeys-0.1.4.tar.gz` & `tmp/global_hotkeys-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_hotkeys-0.1.4.tar", last modified: Wed Jun 21 13:10:57 2023, max compression
+gzip compressed data, was "global_hotkeys-0.1.5.tar", last modified: Wed Jun 21 13:49:00 2023, max compression
```

## Comparing `global_hotkeys-0.1.4.tar` & `global_hotkeys-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:10:57.694508 global_hotkeys-0.1.4/
--rw-rw-rw-   0        0        0     1403 2023-05-29 03:25:19.000000 global_hotkeys-0.1.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     9662 2023-06-21 13:10:57.694508 global_hotkeys-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     7725 2023-06-21 13:08:54.000000 global_hotkeys-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 13:10:57.665789 global_hotkeys-0.1.4/global_hotkeys/
--rw-rw-rw-   0        0        0     4320 2023-06-21 12:57:14.000000 global_hotkeys-0.1.4/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0    10304 2023-06-21 12:58:55.000000 global_hotkeys-0.1.4/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.4/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:10:57.679529 global_hotkeys-0.1.4/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0     9662 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 13:10:57.694508 global_hotkeys-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-06-21 13:09:57.000000 global_hotkeys-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:10:57.692528 global_hotkeys-0.1.4/tests/
--rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.4/tests/_t.py
--rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.4/tests/global_snippets.py
--rw-rw-rw-   0        0        0     2091 2023-06-21 13:05:55.000000 global_hotkeys-0.1.4/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:49:00.419581 global_hotkeys-0.1.5/
+-rw-rw-rw-   0        0        0     1403 2023-05-29 03:25:19.000000 global_hotkeys-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9728 2023-06-21 13:49:00.419581 global_hotkeys-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7791 2023-06-21 13:13:54.000000 global_hotkeys-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 13:49:00.403581 global_hotkeys-0.1.5/global_hotkeys/
+-rw-rw-rw-   0        0        0     4476 2023-06-21 13:47:36.000000 global_hotkeys-0.1.5/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0    10304 2023-06-21 12:58:55.000000 global_hotkeys-0.1.5/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.5/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:49:00.416581 global_hotkeys-0.1.5/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0     9728 2023-06-21 13:49:00.000000 global_hotkeys-0.1.5/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-06-21 13:49:00.000000 global_hotkeys-0.1.5/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:49:00.000000 global_hotkeys-0.1.5/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 13:49:00.000000 global_hotkeys-0.1.5/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 13:49:00.000000 global_hotkeys-0.1.5/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:49:00.419581 global_hotkeys-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-06-21 13:47:45.000000 global_hotkeys-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:49:00.418581 global_hotkeys-0.1.5/tests/
+-rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.5/tests/_t.py
+-rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.5/tests/global_snippets.py
+-rw-rw-rw-   0        0        0     2091 2023-06-21 13:05:55.000000 global_hotkeys-0.1.5/tests/test.py
```

### Comparing `global_hotkeys-0.1.4/CHANGELOG.txt` & `global_hotkeys-0.1.5/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.4/LICENSE.txt` & `global_hotkeys-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.4/PKG-INFO` & `global_hotkeys-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global_hotkeys
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -64,15 +64,22 @@
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["control + 6", None, print_with_params, False, {"test":5}],
-    ["control + 8", press_with_params, release_with_params, False, {"press_param":"pressed!"}, {"release_param": "released!"}],
+    [
+        "control + 8", 
+        press_with_params, 
+        release_with_params, 
+        False, 
+        {"press_param":"pressed!"}, 
+        {"release_param": "released!"}
+    ],
     # dict style
     {
         "hotkey": "control + 4",
         "on_press_callback": None,
         "on_release_callback": print_with_params,
         "actuate_on_partial_release": False,
         "callback_params": {"test": "testing"},
```

### Comparing `global_hotkeys-0.1.4/README.md` & `global_hotkeys-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,22 @@
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["control + 6", None, print_with_params, False, {"test":5}],
-    ["control + 8", press_with_params, release_with_params, False, {"press_param":"pressed!"}, {"release_param": "released!"}],
+    [
+        "control + 8", 
+        press_with_params, 
+        release_with_params, 
+        False, 
+        {"press_param":"pressed!"}, 
+        {"release_param": "released!"}
+    ],
     # dict style
     {
         "hotkey": "control + 4",
         "on_press_callback": None,
         "on_release_callback": print_with_params,
         "actuate_on_partial_release": False,
         "callback_params": {"test": "testing"},
```

### Comparing `global_hotkeys-0.1.4/global_hotkeys/__init__.py` & `global_hotkeys-0.1.5/global_hotkeys/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,19 +47,20 @@
         if "release_callback_params" in binding_raw:
             release_params = binding_raw["release_callback_params"]
         return [_binding, keydown_function, keyup_function, actuate_on_partial_release, press_params, release_params]
     else:
         binding_raw_str = str(binding_raw)
         raise Exception(f"Binding {binding_raw_str} is not the correct_type")
 
-def register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release = False, press_params = None, release_params = 0):
+def register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release = False, press_params = None, release_params = "0e7ef7c6-d3dc-4947-9d7c-5a8f7eb3e1e9"):
     _syntax_check(binding)
     press__params = press_params
     release__params = press_params
-    if release_params != 0:
+    # Using a UUID here as a workaround to differentiate from None being passed.
+    if release_params != "0e7ef7c6-d3dc-4947-9d7c-5a8f7eb3e1e9":
         release__params = release_params
     return hotkey_checker.register_hotkey([hotkey.split("+") for hotkey in binding.replace(" ","").split(",")], press_callback, release_callback, actuate_on_partial_release, press__params, release__params)
  
 def _register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release, press_params, release_params):
 	return hotkey_checker.register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release, press_params, release_params)
 
 def remove_hotkey(binding):
```

### Comparing `global_hotkeys-0.1.4/global_hotkeys/hotkey_checker.py` & `global_hotkeys-0.1.5/global_hotkeys/hotkey_checker.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.4/global_hotkeys/keycodes.py` & `global_hotkeys-0.1.5/global_hotkeys/keycodes.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.4/global_hotkeys.egg-info/PKG-INFO` & `global_hotkeys-0.1.5/global_hotkeys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global-hotkeys
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -64,15 +64,22 @@
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["control + 6", None, print_with_params, False, {"test":5}],
-    ["control + 8", press_with_params, release_with_params, False, {"press_param":"pressed!"}, {"release_param": "released!"}],
+    [
+        "control + 8", 
+        press_with_params, 
+        release_with_params, 
+        False, 
+        {"press_param":"pressed!"}, 
+        {"release_param": "released!"}
+    ],
     # dict style
     {
         "hotkey": "control + 4",
         "on_press_callback": None,
         "on_release_callback": print_with_params,
         "actuate_on_partial_release": False,
         "callback_params": {"test": "testing"},
```

### Comparing `global_hotkeys-0.1.4/setup.py` & `global_hotkeys-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='global_hotkeys',
-  version='0.1.4',
+  version='0.1.5',
   description='',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/btsdev',
   author='btsdev',
   author_email='btsdevman@gmail.com',
   license='MIT',
```

### Comparing `global_hotkeys-0.1.4/tests/global_snippets.py` & `global_hotkeys-0.1.5/tests/global_snippets.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.4/tests/test.py` & `global_hotkeys-0.1.5/tests/test.py`

 * *Files identical despite different names*

